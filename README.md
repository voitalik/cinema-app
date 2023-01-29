# :cinema: Cinema-app

<!-- TOC -->
* [Cinema-app](#cinema-cinema-app)
    * [*Description*](#books-description)
    * [*Features*](#key-features)
    * [*Technologies*](#movie_camera-technologies-list)
    * [*Instructions*](#clapper-how-to-run-project)
<!-- TOC -->





### :books: *Description*
This is a simple cinema web application that allows you to register and authenticate users with different roles, 
add movies, and provide ordering tickets that are stored in shopping carts.
The application is designed following REST, and CRUD and is based on 3-tier architecture.

------------


### :key: *Features*

------------


* implemented authentication and authorization for users
* register new users
* add new movie/cinema hall/movie session
* find movie according to date
* add tickets to shopping cart
* complete orders
* show order history by user

In the application are presented roles ADMIN and USER and implemented following endpoints:

| **Http method** | **Endpoint**                   | **Roles**  | **Description**                                               |
|-----------------|--------------------------------|------------|---------------------------------------------------------------|
| POST            | /register                      | all        | register new user with email and password                     |
| POST            | /cinema-halls                  | ADMIN      | add new cinema hall with capacity and description             |
| POST            | /movies                        | ADMIN      | add new movie with title and description                      |
| POST            | /movie-sessions                | ADMIN      | add new movie session with movieId, cinemaHallId and showTime |
| PUT             | /movie-sessions/{id}           | ADMIN      | update movie session                                          |
| DELETE          | /movie-sessions/{id}           | ADMIN      | delete movie session                                          |
| GET             | /users/by-email                | ADMIN      | get user by email                                             |
| POST            | /orders/complete               | USER       | complete order - tickets from shopping cart moves to order    |
| PUT             | /shopping-carts/movie-sessions | USER       | add tickets to shopping cart                                  |
| GET             | /orders                        | USER       | get user's order history                                      |
| GET             | /shopping-carts/by-user        | USER       | get user's shopping cart                                      |
| GET             | /movie-sessions/available      | ADMIN/USER | get available movie session by id and showtime                |
| GET             | /movies                        | ADMIN/USER | get all movies                                                |
| GET             | /cinema-halls                  | ADMIN/USER | get all cinema halls                                          |

------------


### :movie_camera: *Technologies list*

------------

- Java 11
- Tomcat
- MySQL
- Maven
- Spring framework
- Hibernate


------------

### :clapper: *How to run project*

##### Requirements
- Java 11
- Tomcat 9.0.50
- MySQL 8.0.30

Instruction to compile and launch the application.
1. Clone project from repository.
2. Setup connection attributes to your database into **src/main/resources/db.properties** file.
3. Configure Tomcat server: add artifact for deploying.
4. Run Tomcat configuration.

You can test the app at [http://cinema.eu-west-3.elasticbeanstalk.com](http://cinema.eu-west-3.elasticbeanstalk.com)
