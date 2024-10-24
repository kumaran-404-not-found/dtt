# Use an official OpenJDK runtime as a base image
FROM openjdk:11-jre-slim

# Add a volume to store logs
VOLUME /tmp

# Copy the packaged JAR file into the Docker container
COPY target/myapp.jar myapp.jar

# Expose the port your app runs on
EXPOSE 3000

# Run the JAR file
ENTRYPOINT ["java","-jar","/myapp.jar"]
