![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

![lang](https://img.shields.io/github/languages/top/imanmansour86/E-Commerce-Back-End)
![repo size](https://img.shields.io/github/repo-size/imanmansour86/E-Commerce-Back-End)
![last commit](https://img.shields.io/github/last-commit/imanmansour86/E-Commerce-Back-End)

# E-Commerce-Back-End

## Description

In this app, a backend was built for an e-commerce site. Using Sequelize to interact with a MySQL database and Express.js API, we can GET, PUT, POST and DELETE from the database's tables. The database has the following tables: Category, Product, Tag and ProductTag as an association table. The routes were tested using Insomnia Core.

## Table of Contents

- [E-Commerce-Back-End](#e-commerce-back-end)
  - [Description](#description)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Demo](#demo)
  - [Features](#features)
  - [Tests](#tests)
  - [Built With](#built-with)
  - [Resources Used](#resources-used)
  - [Author](#author)
  - [License](#license)

## Installation

- Go to the app's [repo](https://github.com/imanmansour86/E-Commerce-Back-End) in github and clone the app
- Open the app in VS code, navigate to .env file, change the DB_USER and DB_PW based on current user configurations
- From terminal: navigate to app's directoty and run:

  ```md
  $ npm install
  ```

- From terminal: navigate to db folder in the app's directoty and run:

  ```md
  $ mysql -uroot - p
  ```

- Run the schema file:

  ```md
  source schema.sql
  ```

- From terminal: navigate to the app's directoty and run:

  ```md
  $ npm run seed
  ```

- To invoke the app from terminal, run:

  ```md
  $ node server.js
  ```

## Usage

Below are some screenshots demonstrating testing the routes in Insomnia

GET routes

- Categroy

![Category](./images/get_cat.png)

- Product

![Product](./images/get_product.png)

- Tag

![Tag](./images/get_tag.png)

POST routes

- Categroy

![Category](./images/post_cat.png)

- Product

![Product](./images/post_product.png)

- Tag

![Tag](./images/post_tag.png)

PUT routes

- Categroy

![Category](./images/put_category.png)

- Product

![Product](./images/put_product.png)

- Tag

![Tag](./images/put_tag.png)

## Demo

- [Demo Link](https://watch.screencastify.com/v/YruzCamHF8gX4kTiYpwI)

## Features

The tables have association established in Sequelize models to create the following relationships: Product belongs to Category, and Category has many Product models. Product belongs to many Tag models, and Tag belongs to many Product models. Products can have multiple tags and tags to have many products by using a ProductTag model.

## Tests

To test the functionality of the routes, open Insomnia, specifiy the method in the request and enter the URL to be tested: Sincd the app uses app router, to GET routes for all the categories for example, enter URL http://localhost:3001/api/categories/ and hit send. The GET all products URL is http://localhost:3001/api/products, and GET all tags URL is http://localhost:3001/api/tags

## Built With

- [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [Expressjs](https://expressjs.com/)
- [Sequelize](https://sequelize.org/)
- [MySQL2](https://www.npmjs.com/package/mysql2)
- [dotenv](https://www.npmjs.com/package/dotenv)

## Resources Used

- [W3schools](https://www.w3schools.com)
- [stackoverflow](https://stackoverflow.com)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)

## Author

Iman Mansour

- [Portfolio](https://imanmansour86.github.io/new-portfolio/)
- [Github](https://github.com/imanmansour86)
- [LinkedIn](https://www.linkedin.com/in/iman-mansour-51391515/)
- [Email](mailto:imanmansour86@gmail.com)

## License

This project is licensed under the MIT License
