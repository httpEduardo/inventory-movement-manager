# Inventory Movement Manager

![Java](https://img.shields.io/badge/Java-11-ED8B00?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-REST%20API-6DB33F?logo=springboot&logoColor=white)

A small inventory movement application with a Spring Boot API and a lightweight browser interface. The API stores manual product movements with a date, description, value, and user reference.

## Run the API

From the repository root, start the Spring Boot application with Maven:

```bash
mvn spring-boot:run
```

The API listens on `http://localhost:8080`.

## Endpoint

`GET /movimentos` returns the recorded manual movements as JSON. Each record includes product details, movement date, value, and user reference.

```bash
curl http://localhost:8080/movimentos
```

The `frontend/` directory contains the form markup and JavaScript used by the browser interface.
