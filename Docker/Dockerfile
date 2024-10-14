# Use a base image with Java installed
FROM openjdk:11-jre-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the built jar from the target folder (assuming Maven builds to target/)
COPY target/*.jar app.jar

# Expose the port that the application will use (if applicable)
EXPOSE 8080

# Define the entrypoint to run the jar file
ENTRYPOINT ["java", "-jar", "app.jar"]
