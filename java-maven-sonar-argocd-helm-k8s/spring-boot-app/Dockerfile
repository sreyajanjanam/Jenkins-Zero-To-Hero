# Use Java 17 runtime for Spring Boot app
FROM eclipse-temurin:17-jre-alpine

# Path to the JAR artifact
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the built JAR into the container
COPY ${artifact} app.jar

# Run the Spring Boot application
ENTRYPOINT ["java","-jar","app.jar"]
