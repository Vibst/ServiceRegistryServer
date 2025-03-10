# # Use an official OpenJDK runtime as a parent image
# FROM openjdk:17-jdk-slim

# # Set the working directory in the container
# WORKDIR /app

# # Copy the JAR file into the container
# COPY target/*.jar app.jar


# # Expose the port your Spring Boot application will run on (e.g., 8761)
# EXPOSE 8761

# # Run the JAR file
# ENTRYPOINT ["java", "-jar", "service-registry.jar"]
FROM openjdk:17-jdk-slim
VOLUME /tmp
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]


