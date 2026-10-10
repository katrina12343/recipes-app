# Recipes App

Веб-приложение «Мои рецепты» на стеке PHP + Nginx + MySQL в Docker.

## Запуск

1. Скопировать `.env.example` в `.env`
2. Выполнить `docker compose up -d --build`
3. Открыть http://localhost:8080

## Подключение к БД

- Host: localhost
- Port: 3308
- Database / User / Password — из `.env`

## Остановка

`docker compose down` (данные сохраняются)
`docker compose down -v` (данные удаляются)