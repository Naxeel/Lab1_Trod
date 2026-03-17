## Лаба по Docker

Простое Todo‑API (список задач) на FastAPI + PostgreSQL. Приложение и база крутятся в двух отдельных контейнерах, поднимаются через `docker-compose`.

### Что есть
- контейнер `app` — веб‑API (FastAPI)
- контейнер `db` — PostgreSQL c инициализацией через `init.sql`
- отдельная docker‑сеть, volume для данных БД, наружу открыт только порт `8000` у приложения

### Как запустить
В корне проекта:
```bash
docker compose up --build
```
API будет доступно на `http://localhost:8000`, документация Swagger — на `http://localhost:8000/docs`.

