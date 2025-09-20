# 🚀 Recipe App (FastAPI + Redis + MongoDB + Docker + Nginx)

Этот проект — pet-project уровня портфолио.  
Он демонстрирует использование **FastAPI** в связке с **Redis** и **MongoDB**, развёрнутых в контейнерах через **Docker Compose** и проксируемых через **Nginx**.

---

## 🔹 Возможности (MVP)
- Регистрация и авторизация пользователей (JWT)
- CRUD-операции для рецептов (MongoDB)
- Кэширование популярных рецептов (Redis)
- Nginx как reverse-proxy
- Docker Compose для развёртывания всех сервисов

---

## 🔹 Стек технологий
- **FastAPI** — современный Python веб-фреймворк
- **MongoDB** — база данных для хранения пользователей и рецептов
- **Redis** — кэш и хранение сессий
- **Nginx** — прокси для веб-приложения
- **Docker Compose** — управление сервисами

---

## 📂 Структура проекта
```text
recipe-app/
│── app/
│   │── main.py          # Точка входа FastAPI
│   │── db.py            # Подключение к MongoDB и Redis
│   │── routes/          # API-маршруты
│   │   ├── auth.py
│   │   ├── recipes.py
│   │   └── comments.py
│── nginx/
│   │── default.conf     # Конфигурация Nginx
│── docker-compose.yml   # Docker Compose
│── Dockerfile           # Dockerfile для FastAPI
│── requirements.txt     # Python зависимости
│── .gitignore           # Игнорируемые файлы для Git
│── README.md            # Описание проекта
