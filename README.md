# Crypto ChatBot

A cryptocurrency chatbot application built with Spring Boot, Angular, PostgreSQL, and OpenAI.

## Technologies

- **Backend**: Spring Boot, Java
- **Frontend**: Angular
- **Database**: PostgreSQL
- **AI**: OpenAI API

## Prerequisites

- Java 17+
- Node.js 18+
- PostgreSQL
- OpenAI API Key

## Setup

### 1. Database
```bash
docker run --name postgres-db -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=1234 -e POSTGRES_DB=dbCryptoCurrency -p 5432:5432 -d postgres:15
```

### 2. Backend
```bash
cd backend
# Add your OpenAI API key to application.properties
mvn spring-boot:run
```

Backend runs on: http://localhost:8074

### 3. Frontend
```bash
cd frontend
npm install
ng serve
```

Frontend runs on: http://localhost:4200

## Configuration

Edit `backend/src/main/resources/application.properties`:
```properties
spring.ai.openai.api-key=YOUR_API_KEY_HERE
spring.datasource.url=jdbc:postgresql://localhost:5432/dbCryptoCurrency
spring.datasource.username=admin
spring.datasource.password=1234
```

## Usage

1. Start PostgreSQL
2. Run backend
3. Run frontend
4. Open http://localhost:4200

## Author

[alhm002](https://github.com/alhm002)
