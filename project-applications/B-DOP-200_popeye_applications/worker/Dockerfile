# Stage 1: Build the application
FROM maven:3.6.3-jdk-11 as builder
WORKDIR /app
COPY . .
RUN mvn clean package

# Stage 2: Create the runtime container
FROM openjdk:11-jre-slim
COPY --from=builder /app/target/worker-jar-with-dependencies.jar /worker.jar
CMD ["java", "-jar", "/worker.jar"]
