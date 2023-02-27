# django-rest-boilerplate

A reusable Django REST Framework boilerplate with JWT authentication, custom user model, and a clean project structure. Built to speed up API project setup at Aayulogic.

## Tech Stack

- Python 3.9
- Django 4.0.4
- Django REST Framework 3.13.1
- SimpleJWT 5.2.0
- PostgreSQL (psycopg2)

## Features

- Custom User model with email as username
- JWT auth (register, login, logout, token refresh)
- Change password endpoint
- Profile view and update
- Django test suite included

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register/` | Register new user |
| POST | `/api/auth/token/` | Login - get JWT tokens |
| POST | `/api/auth/token/refresh/` | Refresh access token |
| POST | `/api/auth/logout/` | Blacklist refresh token |
| GET/PATCH | `/api/auth/profile/` | Get or update profile |
| POST | `/api/auth/change-password/` | Change password |

## Setup

```bash
pip install -r requirements.txt
cp .env.example .env
python manage.py migrate
python manage.py runserver
```

## Running Tests

```bash
python manage.py test app.tests
```
# readme
