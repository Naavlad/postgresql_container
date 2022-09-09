![](https://img.shields.io/github/license/Naavlad/postgresql_container?style=flat-square)
# База PosqreSQL

Для параллельного развертывания на одном сервере контейнеров по имени проекта

## Stack

- PosqreSQL

## Подготовка к запуску

git clone [https://github.com/Naavlad/postgresql_container.git](https://github.com/Naavlad/postgresql_container.git)

Переименовать файл .env.dev в .env и указать в нем недостающую информацию

`COMPOSE_PROJECT_NAME` - Будет использоваться как POSTGRES_DB  
`EXTERNAL_PORT` - внешний порт(может быть несколько для разных контейнеров)

Если несколько ```docker-compose``` расскоментировать ```networks```
и указать внутреннюю сеть

`NETWORK` - Внутренняя сеть сервера для нескольких docker-compose

```bash
COMPOSE_PROJECT_NAME= <Название проекта>
EXTERNAL_PORT= <внешний порт>

NETWORK=<сеть>

POSTGRES_USER=
POSTGRES_PASSWORD=
```
