# :cinema: Cinema-app

<!-- TOC -->
* [Cinema-app](#Cinema-app)
    * [*Description*](#description)
    * [*Features*](#features)
    * [*Technologies*](#technologies)
    * [*Instructions*](#instructions)
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

##### Requirenments
- Java 11
- Tomcat 9.0.50
- MySQL 8.0.30

Instruction to compile and launch the application.
1. Clone project from repository.
2. Setup connection attributes to your database into **src/main/resources/db.properties** file.
3. Configure Tomcat server: add artifact for deploying.
4. Run Tomcat configuration.
