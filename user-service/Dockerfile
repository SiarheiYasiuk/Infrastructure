FROM openjdk:17-jdk-slim
ARG JAR_FILE=target/*.jar
RUN apt-get update && apt-get install -y curl && rm -rf /var/lib/apt/lists/*
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]