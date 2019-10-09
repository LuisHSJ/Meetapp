<h1 align="center">
    <img alt="Go Stack - Meetapp logo" src="https://res.cloudinary.com/lukemorales/image/upload/v1567376018/readme_logos/meetapp_mljojp.png"/>
    <br>
    Bootcamp Rocketseat - Desafio Meetapp
</h1>

<h4 align="center">
  Realização de Desafio Final para certificação
</h4>

<p align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/LuisHSJ/Meetapp.svg">

  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/LuisHSJ/Meetapp.svg">

<a href="https://www.codacy.com/manual/LuisHSJ/Meetapp?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=LuisHSJ/Meetapp&amp;utm_campaign=Badge_Grade">
  <img src="https://api.codacy.com/project/badge/Grade/b5a5c4232f0543d791afff53225d0273"/></a>

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/LuisHSJ/Meetapp.svg">
  <a href="https://github.com/LuisHSJ/Meetapp/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/LuisHSJ/Meetapp.svg">
  </a>

  <img alt="GitHub" src="https://img.shields.io/github/license/LuisHSJ/Meetapp.svg">
</p>

________________________________________________________________________________________________________________________________________

## Execução - Backend


```bash
docker run --name postgres -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
docker run --name redis -p 6379:6379 -d -t redis:alpine
```

Criar o banco de dados se ainda não tiver sido criado

```bash
cp .env.example .env.example .env e defina as variáveis corretas, incluindo a APP_URL se você não quiser usar http://localhost:3333
```

Instalar as dependências e executar as migrações do banco de dados

```bash
yarn install && yarn sequelize db:migrate
```

Por fim, execute o servidor e a fila

* Servidor: yarn dev
* Fila: yarn queue

________________________________________________________________________________________________________________________________________

## Execução - Frontend

Defina o url da api em src/services/api.js se você não quiser usar http://localhost:3333

Instale as dependências do frontend e inicie o servidor

* yarn install
* yarn start

________________________________________________________________________________________________________________________________________

## Execução - Mobile

Defina o url da api em src/services/api.js se você não quiser usar http://localhost:3333

Instale as dependências do mobile e inicie o emulador 
* yarn install

Para execução em dispositivo iOS: 
* react-native run-ios

Para execução em dispositivo Android:
* react-native run-android

________________________________________________________________________________________________________________________________________

## License
[MIT](https://github.com/LuisHSJ/Meetapp/blob/master/LICENSE)
