# Запуск в dev окружении
1) cd dev

docker compose up -d

# Запуск в prod окружении
2) cd prod

docker compose up -d

# Настройка
Скопировать файл `.env.example` в `.env` и заполнить его:

1. POSTGRES_USER - Логин пользователя в бд;
2. POSTGRES_PASSWORD - Пароль пользователя в бд;
3. POSTGRES_DB - Название базы данных;
4. POSTGRES_HOST- Хост для бд(Если в докере, то указывать `db`);
5. NGINX_PORT - порт для веб-сервера;
7. POSTGRES_PORT - порт для базы данных.