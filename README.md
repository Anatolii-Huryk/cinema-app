# Cinema-app
___

## Introduction

This is a prototype of a web application that works like a movie theater.
In this application, user can have two roles `ADMIN` or `USER`.
___

## Project structure

#### The structure of this project consists of 3 levels:
* Data access layer (DAO).
* Application layer (service).
* Presentation layer (controllers).

___

## Opportunities depending on the role
There are two ready-made users provided for testing this application:
- ADMIN
- USER

You can register (POST: /register)

Admin:
* POST: /cinema-halls
* POST: /movies
* POST: /movie-sessions
* PUT: /movie-sessions/{id}
* DELETE: /movie-sessions/{id}
* GET: /users/by-email

User:
* POST: /orders/complete 
* PUT: /shopping-carts/movie-sessions 
* GET: /orders
* GET: /shopping-carts/by-user
* GET: /cinema-halls
* GET: /movies
* GET: /movie-sessions/available
___
### Technologies:
* MySql
* Hibernate ORM
* Spring(Core, Web, Security)
* Apache Tomcat
* Maven
* JSON
___
## How to start the application

1. Configure Apache Tomcat
2. Install MySQL with MySQL Workbench
3. Fork this project on GitHub
4. In the db.properties change YOUR_URL, YOUR_USERNAME and YOUR_PASSWORD values
to the ones you specified when installing MySQL, also change JDBC_DRIVER
5. Run the application
