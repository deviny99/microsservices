FROM openjdk:11-jdk
MAINTAINER Marcos Rocha
WORKDIR /app
COPY /target/*.jar /app/app.jar
ENV DISCOVERY_HOST=localhost
ENV PORT=8080
ENTRYPOINT ["java","-Dspring.profiles.active=prod", "-jar", "app.jar"]
EXPOSE ${PORT}