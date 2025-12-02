# 🚀 Hello World Spring Boot Application – Dockerized

A minimal Spring Boot REST API packaged inside a Docker container.  
This project demonstrates how to run a simple Java application using Docker and Eclipse Temurin (Java 21).

---

## 📌 Endpoint
GET http://localhost:8080/home/api

## 📌 Response
Hello World


---

## 🛠️ Tech Stack

- Spring Boot  
- Java 21 (Eclipse Temurin)  
- Docker  
- REST API  

---

## 📦 Dockerfile

```dockerfile
FROM eclipse-temurin:21
COPY Hello-World-0.0.1-SNAPSHOT.jar Hello-World.jar
ENTRYPOINT ["java", "-jar", "Hello-World.jar"]
```

## 🐳 Run Using DockerHub Image

You can directly pull and run the image from DockerHub without building anything locally.

### 1️⃣ Pull the Image**
```bash
docker pull zunaidhossain/spring-hello-world:v1
```


### 2️⃣ Run the Container
```bash
http://localhost:8080/home/api
```

### 3️⃣ Access the API
```bash
docker run -p 8080:8080 zunaidhossain/spring-hello-world:v1
```
