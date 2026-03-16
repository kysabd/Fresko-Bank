# FreskoBank

Мини-банк (frontend + backend)

## Структура

- `frontend/` — HTML+CSS входная панель, статический UI
  - `index.html`
  - `styles.css`
- `backend/` — Java/Maven каркас
  - `pom.xml`
  - `src/main/java/com/freskobank/App.java`

## Запуск

1. Фронтенд: открыть `frontend/index.html` в браузере.
2. Бэкенд: `cd backend && mvn compile exec:java -Dexec.mainClass=com.freskobank.App` (или `mvn package && java -jar target/backend-0.1.0-SNAPSHOT.jar`).

## Дальше

- интегрировать Spring Boot, добавить API `/login`, хранилище (PostgreSQL/H2), Docker Compose.
- сделать проверки логина на фронте и AJAX-вызовы к бэкенду.
