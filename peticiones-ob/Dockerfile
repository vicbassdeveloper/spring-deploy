FROM openjdk:latest
LABEL authors="alex"
COPY /target/sprin-deploy-1.0.jar spring-deploy.jar
ENTRYPOINT ["java", "-jar", "/spring-deploy.jar"]