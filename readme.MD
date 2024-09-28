
---
# SimpleRestService

## Overview

This project is a basic RESTful web service built using Spring Boot. It demonstrates the creation of REST endpoints and provides a simple greeting service. The project is designed to introduce you to the fundamentals of Spring Boot and RESTful web services.

## Features

- Stand-alone Spring application
- Embedded Tomcat server
- RESTful endpoint to return greetings
- Customizable greetings with query parameters

## Prerequisites

- Java 11 or above
- Maven
- An IDE (e.g., IntelliJ IDEA, Eclipse)
- A REST client (e.g., Postman) for testing

## Project Setup

### Step 1: Initialize the Project

1. Go to [Spring Initializr](https://start.spring.io/).
2. Set the following configurations:
    - **Project**: Maven Project
    - **Language**: Java
    - **Spring Boot**: 2.7.0 (or the latest stable version)
    - **Group**: `com.example`
    - **Artifact**: `simple-rest-service`
    - **Name**: `SimpleRestService`
    - **Package Name**: `com.example.simplerestservice`
    - **Packaging**: Jar
    - **Java**: 11 (or your installed version)
3. Add the dependency:
    - **Spring Web**
4. Click "Generate" to download the project and unzip it.

### Step 2: Import the Project

1. Open your IDE.
2. Import the unzipped project as a Maven project.

## Running the Application

1. Build the executable JAR file using the command: ```mvn clean package```
2. Navigate to the project directory in your terminal and Execute the following command: ```mvn spring-boot:run```
OR
1. Ensure that the `SimpleRestServiceApplication` class is located in the `src/main/java/com/example/simplerestservice` package. 2.
2. Run the `SimpleRestServiceApplication` class.
3. The application will start on the default port `8080`.

## Testing the RESTful Web Service

1. Open Postman or any other REST client.
2. Make a GET request to `http://localhost:8080/greeting`.
    - You should receive a JSON response similar to:
      ```json
      {
        "id": 1,
        "content": "Hello, World!"
      }
      ```
3. Test with a query parameter by making a request to `http://localhost:8080/greeting?name=John`.
    - You should receive a JSON response similar to:
      ```json
      {
        "id": 2,
        "content": "Hello, John!"
      }
      ```

---
