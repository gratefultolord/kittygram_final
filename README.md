# Kittygram final

## Описание
Данный проект представляет собой площадку для публикации данных о котах, включая их имя, год рождения, цвет, владельца и достижения.

**Инструменты и стек:** #Python #Django #Docker-compose #API #Nginx #Pillow #Djoser #Gunicorn #Python-dotenv #JSON #YAML #Postman #PyCharm

## Запуск
Для запуска приложения необходим сервер, рассмотрим на примере сервера под управлением ОС Linux.

1. Подготовим виртуальное окружение в директории проекта создадим файл .env:
```bash
nano .env
```

2. Добавляем следующие переменные:
```nano
POSTGRES_DB=kittygram
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
DB_HOST=127.0.0.1
DB_PORT=5432
SECRET_KEY=...
```

3. Устанавливаем к Docker утилиту Docker Compose:
```bash
sudo apt update
sudo apt-get install docker-compose-plugin 
```

4. В директорию проекта копируем файл `docker-compose.production.yml` и запускаем Docker Compose:
```bash
sudo docker-compose up -f docker-compose.production.yml up
```

## Примеры запросов

Добавить питомца: POST `/cats/add`

Редактировать питомца: PUTCH `/cats/edit`

Просмотр питомца: GET `/cats/{cat_id}`


## Статус репозитория

Workflow: ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/gratefultolord/kittygram_final/main.yml)


## Об авторе
Python-разработчик
>[gratefultolord]([https://github.com/gratefultolord])