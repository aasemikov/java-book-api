# Books Management API - Отчет о тестировании

## Описание проекта

Spring Boot приложение для управления книгами с использованием Spring Web, Spring Data JPA и H2 database.

## Технологии

-   Java 17
-   Spring Boot 3.5.7
-   Spring Data JPA
-   H2 Database
-   Gradle

## Запуск приложения

```bash
./gradlew bootRun
```
Приложение будет доступно по адресу: `http://localhost:8080`

## API Endpoints

| Метод | Endpoint | Описание |
|-------|----------|-----------|
| GET | `/api/books` | Получить все книги |
| GET | `/api/books/{id}` | Получить книгу по ID |
| POST | `/api/books` | Создать новую книгу |
| PUT | `/api/books/{id}` | Обновить книгу |
| DELETE | `/api/books/{id}` | Удалить книгу |

## Тестирование API endpoints

### 1. GET /api/books - Пустой список

Запрос: `GET http://localhost:8080/api/books`

![GET http://localhost:8080/api/books](https://github.com/aasemikov/java-book-api/raw/main/report/img/1.png)

### 2. POST /api/books - Создание первой книги

Запрос: `POST http://localhost:8080/api/books`

![POST http://localhost:8080/api/books](https://github.com/aasemikov/java-book-api/raw/main/report/img/2.png)

### 3. POST /api/books - Создание второй книги

Запрос: `POST http://localhost:8080/api/books`

![POST http://localhost:8080/api/books](https://github.com/aasemikov/java-book-api/raw/main/report/img/3.png)

### 4. GET /api/books - Список всех книг

Запрос: `GET http://localhost:8080/api/books`

![GET http://localhost:8080/api/books](https://github.com/aasemikov/java-book-api/raw/main/report/img/4.png)


### 5. GET /api/books/1 - Получить книгу по ID

Запрос: `GET http://localhost:8080/api/books/1`

![GET http://localhost:8080/api/books/1](https://github.com/aasemikov/java-book-api/raw/main/report/img/5.png)

### 6. PUT /api/books/1 - Обновить книгу

Запрос: `PUT http://localhost:8080/api/books/1`

![PUT http://localhost:8080/api/books/1](https://github.com/aasemikov/java-book-api/raw/main/report/img/6.png)

### 7. DELETE /api/books/2 - Удалить книгу

Запрос: `DELETE http://localhost:8080/api/books/2`

![DELETE http://localhost:8080/api/books/2](https://github.com/aasemikov/java-book-api/raw/main/report/img/7.png)

### 8. GET /api/books/2 - Проверка удаления

Запрос: `GET http://localhost:8080/api/books/2`

![GET http://localhost:8080/api/books/2](https://github.com/aasemikov/java-book-api/raw/main/report/img/8.png)