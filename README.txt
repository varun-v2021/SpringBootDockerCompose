https://javatodev.com/docker-compose-for-spring-boot-with-mysql/

The following line in docker-compose.yml doesnt make a difference whether its present or not
command: sh -c './wait-for mysql_db:3306 -- npm start'