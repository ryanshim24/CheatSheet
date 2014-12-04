STARTING OUT YOUR APPS
============

## Node APPS

### Starting off

* mkdir firstapp (get the party started)
* touch app.js
* touch .gitignore
* git init

Add the text 'node_modules' in our .gitignore

* echo "node_modules" >> .gitignore

Start the project and start adding dependencies that you might need!

* npm init
* Ex) npm install --save express ejs pg lodash sequelize sequelize-cli

If your going to incoporate database create one and sequelize the project

* createdb firstapp
* sqlize init

### Setup - config, models and migrations

change config file to

```
{
  "development": {
    "database": "firstapp",
    "host": "127.0.0.1",
    "dialect": "postgres"
  },
  "test": {
    "database": "database_test",
    "host": "127.0.0.1",
    "dialect": "postgres"
  },
  "production": {
    "database": "database_production",
    "host": "127.0.0.1",
    "dialect": "postgres"
  }
}

```