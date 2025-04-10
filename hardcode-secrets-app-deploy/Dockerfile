# 1. Use an official slim version of OpenJDK 17 as the base image
FROM openjdk:17-jdk-slim

# 2. Set the working directory inside the container to /app
WORKDIR /app

# 3. Copy the built JAR file from your local machine into the container
COPY target/demo-0.0.1-SNAPSHOT.jar app.jar

# 4. Set the AWS region (you can override this using Kubernetes environment variables)
ENV AWS_REGION=us-east-2

# 5. Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "app.jar"]
