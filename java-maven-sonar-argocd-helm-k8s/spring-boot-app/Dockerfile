# Use the current, supported base image
FROM eclipse-temurin:11-jre-alpine

# Use build argument for the artifact path
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the JAR file into the container
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
