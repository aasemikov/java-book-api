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

![GET http://localhost:8080/api/books](https://github.com/aasemikov/{java-book-api}/raw/main/report/img/1.png)