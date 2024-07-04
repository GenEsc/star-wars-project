# Use an openjdk image as the base image
FROM openjdk:17-jdk-slim

# Set the working directory
WORKDIR /app

# Copy the backend application JAR file
COPY star-wars/target/star-wars-0.0.1-SNAPSHOT.jar /app/backend-app.jar

# Expose port 8080 (or the port your backend service listens on)
EXPOSE 8080

# Run the application
CMD ["java", "-jar", "/app/backend-app.jar"]