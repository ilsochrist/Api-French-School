# SCHOOL FRENCH API

This repository contains the REST API with NodeJS from a French school, some activities were carried out:
 
 - JSON-type data structures were generated with useful information for the user.
 - Added "Paranoid" option for smooth deletion
 - Migrations were created to add columns to tables
 - Created deletedAt columns to use soft delete feature
 - Restored deleted records via soft deletion, using .restore()

### Used tools to create the api:

 - NodeJs
 - Express
 - Sequelize
 - Body Parser
 - Nodemon


### How to use the api.
Make a copy of the repository and inside the backend folder run the following command:
```sh
npm install
npm run dev
```
or
```sh
yarn install
yarn dev
```

Create a database with MySQL:
```sh
create database school_frances
```
Now to perform the migrations and seeds, open the terminal again inside the backend folder and type:
```sh
npx sequelize-cli db:create
npx sequelize-cli db:migrate
npx sequelize-cli db:seed:all
```
or
```sh
yarn sequelize db:create
yarn sequelize db:migrate
yarn sequelize db:seed:all
```
