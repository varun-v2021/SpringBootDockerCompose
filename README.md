# Spring Boot MySQL Base Project

This application was developed to demonstrate Spring Boot with MySQL with simple API.

Technologies Used

- Spring Boot 2.4.1
- Spring Data JPA
- Lombok
- MySQL

How to Run this application using docker compose

Running Spring Boot Application and MySQL Database Using Docker Compose

Now we have our docker compose setup for this application. So first create a jar build for this application using the following command,

Navigate to application root folder and execute,

$ ./gradlew clean build

Now there should be a newly created jar file with all the necessary files to run this application on build/libs folder.

Then create the build with docker compose to build docker image using built jar file.

$ docker-compose build

Then use following command to run whole setup using docker compose.

$ docker-compose up

Then It will capture the docker-compose.yml and start running using the instructions given on that file.

How to Run this application as standalone spring boot

First change the **src/main/resources/application.properties** with your MySQL instance properties.

Then,

```shell
$ ./gradlew bootRun
```

or create a build using following command,

```shell
$ ./gradlew clean build
```

Then start the JAR file using java

```shell
$ java -jar build/libs/spring-boot-mysql-base-project-0.0.1-SNAPSHOT.jar
```

### Reference

https://javatodev.com/docker-compose-for-spring-boot-with-mysql/

