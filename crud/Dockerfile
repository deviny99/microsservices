FROM openjdk:11-jdk
MAINTAINER Marcos Rocha
WORKDIR /app
COPY /target/*.jar /app/app.jar
ENV PORT=8080
ENTRYPOINT ["java","-Dspring.profiles.active=prod", "-jar", "app.jar"]
EXPOSE ${PORT}