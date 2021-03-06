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

User:
GET: /orders (display all the orders)
GET: /shopping-carts/by-user (display the contents of the current user's shopping)
POST: /orders/complete (complete the current order)
PUT: /shopping-carts/movie-sessions (add movie session to the shopping cart)

Admin:
* POST: /cinema-halls (add new cinema hall)
* POST: /movies (add new movie)
* POST: /movie-sessions (add new movie session)
* PUT: /movie-sessions/{id} (update movie session with specified id)
* DELETE: /movie-sessions/{id} (delete movie session by id)
* GET: /users/by-email (find user by email)

User and Admin:
* GET: /cinema-halls (display all the cinema halls)
* GET: /movies (display all the movies)
* GET: /movie-sessions/available (display all the available movie sessions)
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
6. You can test app with credentials of this admin : login - user@gmail.com, password - 1234 . This user is already injected to our app