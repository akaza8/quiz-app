# 📚 Quiz API - Online Quiz Application Backend

A RESTful API for managing online quizzes built with **Spring Boot**, providing endpoints for quiz creation, question management, and quiz-taking functionality.

---

## 📝 Project Description
This Quiz API is a backend service that allows users to:
- Create and manage quizzes
- Add different types of questions (single choice, multiple choice, text-based)
- Take quizzes and receive scores
- View available quizzes

The API follows **RESTful principles** and includes comprehensive validation, error handling, and testing.

---

## ✨ Features

### Core Features
- **Quiz Management**: Create quizzes with custom titles
- **Question Management**: Add questions with multiple choice options
- **Quiz Taking**: Fetch questions and submit answers for scoring
- **Flexible Question Types**: Support for single choice, multiple choice, and text-based questions

### Bonus Features
- List all available quizzes
- Comprehensive validation based on question types
- Swagger UI for API documentation
- H2 in-memory database for easy development

---

## 🛠 Technology Stack
- Java 17
- Spring Boot 3.2.0
- Spring Data JPA
- H2 Database (Development)
- PostgreSQL (Production-ready)
- MapStruct (Object mapping)
- Lombok (Boilerplate reduction)
- Swagger/OpenAPI 3.0 (API documentation)
- Maven (Build tool)

---

## 🚀 Getting Started

### Prerequisites
- Java 17 or higher
- Maven 3.6 or higher
- Git

### Installation

Clone the repository:
```bash
git clone https://github.com/akaza8/quiz-app.git
cd quiz-app
mvn clean install
```
## 2. Run the Application

### Option A: Run with Maven
```bash
mvn spring-boot:run
```
### Option B: Run the JAR file
```bash
java -jar target/quiz-app-0.0.1-SNAPSHOT.jar
```

The application will start at:

- API Base URL → [http://localhost:8080/api](http://localhost:8080/api/quizzes)
- Swagger UI → [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)
- H2 Console → [http://localhost:8080/h2-console](http://localhost:8080/h2-console)  
  (Username: sa, Password: empty)

## 3. Run with Docker

### Build & Run Locally
```bash
docker build -t quiz-app .
docker run -p 8080:8080 quiz-app
```
### Run from Docker Hub
```bash
docker pull akashlawande/quiz-app:latest
docker run -p 8080:8080 akashlawande/quiz-app:latest
```

## 5. API Documentation

- Swagger UI → [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)
- OpenAPI JSON → [http://localhost:8080/v3/api-docs](http://localhost:8080/v3/api-docs)
