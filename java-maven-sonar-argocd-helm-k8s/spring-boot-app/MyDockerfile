# Use a compatible Java 11 runtime base image
FROM eclipse-temurin:11-jre

# Path to the Spring Boot jar
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# Run the jar
ENTRYPOINT ["java", "-jar", "app.jar"]
