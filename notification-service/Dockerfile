FROM eclipse-temurin:17-jdk
WORKDIR /app
RUN apt-get update && apt-get install -y curl && rm -rf /var/lib/apt/lists/*
COPY .env ./
COPY target/*.jar app.jar
ENTRYPOINT ["java","-jar","app.jar"]
