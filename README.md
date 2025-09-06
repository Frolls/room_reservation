# Room Reservation System

Система бронирования переговорных комнат с использованием современных технологий: FastAPI, SQLAlchemy, Alembic и Google Sheets API. Предоставляет RESTful API для управления пользователями, переговорными комнатами и их бронированием.

## Особенности

- Аутентификация пользователей через FastAPI Users
- Управление переговорными комнатами с описанием
- Система бронирования с проверкой конфликта времени
- Интеграция с Google Sheets для автоматического создания отчетов

## Установка

### 1. Клонирование репозитория:

```bash
git clone git@github.com:Frolls/room_reservation.git
cd room_reservation
```

### 2. Создание виртуального окружения:

```bash
# Создание виртуального окружения
python -m venv venv

# Активация виртуального окружения
source venv/bin/activate  # Linux/MacOS
# или
venv\Scripts\activate  # Windows
```

### 3. Установка зависимостей:

```bash
# Все манипуляции должны выполняться в виртуальном окружении
source venv/bin/activate  # Linux/MacOS
# или
venv\Scripts\activate  # Windows

# Установка зависимостей из requirements.txt
pip install -r requirements.txt
```

## Запуск приложения

### Локальный запуск:

```bash
# Все манипуляции должны выполняться в виртуальном окружении
source venv/bin/activate  # Linux/MacOS
# или
venv\Scripts\activate  # Windows

# Создание миграций и применение их к БД
alembic upgrade head

# Запуск сервера
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```

## API документация

Доступна по следующим адресам:
- Swagger UI: http://localhost:8000/docs
- Redoc: http://localhost:8000/redoc

## Используемые технологии

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://python.org/)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
[![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-1.4-blue.svg)](https://www.sqlalchemy.org/)
[![Pydantic](https://img.shields.io/badge/Pydantic-orange.svg)](https://docs.pydantic.dev/)
[![Aiogoogle](https://img.shields.io/badge/Aiogoogle-blue.svg)](https://aiogoogle.readthedocs.io/)
[![Google Sheets API](https://img.shields.io/badge/Google%20Sheets%20API-green.svg)](https://developers.google.com/sheets/api)

## Автор

[Иван Фролов](https://github.com/Frolls)

## Лицензия

MIT License
