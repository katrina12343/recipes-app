# Recipes App — инструкция по развёртыванию

## Требования
- Docker и Docker Compose

## Шаги
1. Распаковать архив.
2. Загрузить образы: `docker load -i recipes-app.tar`
3. Скопировать `.env.example` в `.env`
4. Запустить: `docker compose up -d`
5. Открыть http://localhost:8080

## Если порт занят
Измените в `docker-compose.yml`:
- nginx: `8081:80` вместо `8080:80`
- mysql: `3307:3306` вместо `3306:3306`