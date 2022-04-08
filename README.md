# SpringBoot Social Network Project

- Circle CI build status:
[![CircleCI](https://circleci.com/gh/Prophet1999/Social-Media-App-Backend-SpringBoot.svg?style=svg&circle-token=54d82edd98892db8d4e69740d9bee65e48242495)](https://circleci.com/gh/Prophet1999/Social-Media-App-Backend-SpringBoot)

## Introduction
This project is a continuation of the previous one. The previous project was made with pure Servlets and JSP
 technologies [details here](https://github.com/Prophet1999/Social-Network.git). I used the same
  template layout and created a new project using SpringBoot.

## Functionality
### Base
- Login / Logout
- Register
- View own profile
- View other users profiles
- Send messages
- Add and remove friends
- Accept and decline friends requests
- Update profile information
- Change password
- Search for other users
- View other users friends lists
- View last messages
- Drag and drop profile image upload
- Internationalization: English and Russian languages
- Localization

### Admin
- Make other user admin
- Block user

## Technologies used 
### Stack:
- Java 11
- Spring: SpringBoot, MVC, Data JPA, Security, DevTools, Actuator
- Maven
- H2, Mysql, ClearDb(Heroku)
- Thymeleaf
- Javascript, jQuery
- Html, CSS, Bootstrap
- Test: JUnit, Mockito

### Environment
- Heroku as CD tool
- Circle CI as CI tool
- Docker for containerization

## Application demo is available on Heroku  
Link: [https://springboot-social-network.herokuapp.com/](https://springboot-social-network.herokuapp.com/)  
Cersei is average user and Tyrion Lannister is super admin. Tyrion can't be blocked or made average admin user.

Credentials for Cersei Lannister:
 - login cersei@lannister.ru
 - password fun123  
 
Tyrion Lannister credentials:
 - login tyrion@lannister.ru
 - password fun123
 
 ## Quick start
 
 ### Required:
 - Java 11
 - Maven 
 
 ### Steps:
 1. git clone https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot.git
 2. mvn clean package -DskipTests=true
 3. cd web.social.network/target
 4. java -jar -Dspring.profiles.active=dev social-network.jar
 5. Go to http://localhost:8080

## Application profiles
- dev - profile for development, uses embedded H2 database
- qa - profile for qa testing, uses Mysql either local, or from docker container: [mysql docker container](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/master/docker/mysql%20docker%20commands.md)
- prod - profile for Heroku, uses ClearDb. ClearDb is Heroku analog of Mysql: [details](https://devcenter.heroku.com/articles/cleardb)
- docker - profile for Docker. It is created to test connection between 2 containers: mysql and social-network(spring
 boot app)
 
## Docker
This application is tested in Docker.  
I made 2 containers: mysql and social-network, and then linked them.  
Commands for images creation and containers startup may be found in the directory: [docker](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/tree/master/docker)

## Screenshots
![1](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/1.png)
![2](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/2.png)
![3](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/3.png)
![4](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/4.png)
![5](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/5.png)
![6](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/6.png)
![7](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/7.png)
![8](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/8.png)
![9](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/9.png)
![10](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/10.png)
![11](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/11.png)
![12](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/12.png)
 
### Todo: 
- Improve test coverage. Yes, I know it is very important, but I don't have enough time.

# Social Network Jsp and Servlets Project
Maven multi-module project that simulates social network of Game of Thrones creatures.
Admin user for any profile is Tyrion Lannister as the most smart character. 

Demo may be observer on Heroku by link: [Social Network](https://dcsocial.herokuapp.com).

Tyrion Lannister credentials for login are email: tyrion@adm.ru, password: aaa123.

Heroku disables application if it is not used for a long time(more than 2 hours or more). So it may
take some time for the application initialization and start. 

## Used technologies:
* Java 8 as backend language
* Maven 3.5.4 as build tool
* Servlets 
* Jsp as template engine
* Javascript, jQuery as client-side language/library
* Java API for WebSocket(JSR 356) for notifications
* Bootstrap 3.3.7 framework for UI
* CSS for markup
* Bootstrap-notify plugin for push notifications
* JUnit for unit testing
* Mockito for servlets testing
* Jacoco for checking test coverage
* Git as version control system

## Environment
* Tomcat 8 as web-server
* H2/MySql as data bases - both supported
* Heroku as cloud and deployment tool
* Intellij Idea as IDE

## Features
* Custom / Tomcat connection pool both supported
* DAO pattern for objects access
* Auth filter for security
* Jsp tags
* Bootstrap client-side validation without library
* Drag&Drop avatar image upload without library
* Pagination without library

## Functionality
* Multi-language portal(Ru, En)
* Data initialization on start-up.
* Registration
* Login/Logout
* Administrator user with facilities to block/unblock user or make him(her) admin
* Change user settings(avatar, first name, last name, date of birth,...)
* Messages
* Push notifications about recent messages
* User search by first name and last name 
* Users pagination
* Friends requests and friendship acceptance
* Friends search
* Error page and page for a blocked user

## About the project and its purpose
This project is based on JSP and Servlets technology stack. 
The purpose of the project was to master these core java technologies for web without any framework.

### Profiles
The project has 2 profiles for build: custom and tomcat, by default custom is used.
Depending on the chosen profile the application would use custom connection pool or tomcat connection pool. 

I wanted to train my jdbc skills and write my custom connection pool. Module custom.connection is used for
this. Is is activated by default or explicitly by choosing profile "custom". If choose this profile, than all stub data
will be initialized with all game of thrones characters.

It seemed to me a good idea to have some other module for tomcat connection pool testing. 
Module tomcat.connection is used for this reason, it may be activated by choosing profile "tomcat". 
It was supposed to be a connection that should represent production connection. 
That's why this module will initialize only data base schema and admin user.

### Security
An authorization filter is used for security of the web application. It checks user's session and performs different actions
depending on the data obtained.

For disabling possibility of session hijacking and man in the middle attacks some preferences were written in the web.xml file.
A block "\<session-config\>" contains two lines "\<http-only\>" and "\<secure\>", one of them "\<secure\>" blocks local development
because it requires https connection. It is the reason why it is commented by default, but it supposed to be uncommented in
production environment. Actually, Maven may pack different web.xml file depending on profile used, but I did not want to do this.


### TODO
A lot of things should be done to make this project ready for a real production including testing.
But my aim was to prototype social network project based on Servlets and Jsp technologies. 
I made here everything I wanted to use.

And....I have no time. 

+ move project to SPA(single page application)
+ expand test coverage
+ expand validation and error messages for not only index.jsp page, but also for other pages
+ make a new module for JSON objects requesting and responding. It is a good idea to write something like a custom lib for 
information exchange in JSON format using Jackson or Gson. But it will require to change all templates. 
Additionally, all js code should be updated for parsing and sending json objects.
+ add screenshots of the project and update readme.md
