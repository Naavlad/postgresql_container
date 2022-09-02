![](https://img.shields.io/github/license/Naavlad/postgresql_container)
# База PosqreSQL
Для параллельного развертывания на одном сервере контейнеров по имени проекта

## Stack

- PosqreSQL

## Подготовка к запуску

Переименовать файл .env.dev в .env и указать в нем недостающую информацию

```COMPOSE_PROJECT_NAME``` - Будет использоваться как POSTGRES_DB
```EXTERNAL_PORT``` - внешний порт(может быть несколько для разных контейнеров)

```bash
COMPOSE_PROJECT_NAME= <Название проекта>
EXTERNAL_PORT= <внешний порт>

POSTGRES_USER=
POSTGRES_PASSWORD=
```
