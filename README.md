# База PosqreSQL

## Stack

- PosqreSQL

## Подготовка к запуску

Переименовать файл .env.dev в .env и указать в нем недостающую информацию

`EXTERNAL_PORT` - внешний порт (может быть несколько для разных контейнеров)

- установлен по умолчанию - `5432`

`NETWORK` - Внутренняя сеть сервера для нескольких docker-compose

- по умолчанию создается при запуске `postgres_network`

```bash
# default settings in docker-compose
# EXTERNAL_PORT=5432
# NETWORK=postgres_network
EXTERNAL_PORT=
NETWORK=


# set
POSTGRES_DB=
POSTGRES_USER=
POSTGRES_PASSWORD=
```
