# docker-laravel

Run docker and build:

```bash
docker compose up -d --build
```
Run command line in container:

```bash
docker compose run --rm php /bin/sh
```
Create laravel project via composer:

```bash
docker compose run --rm composer create-project laravel/laravel .
```
If access Forbidden:

```bash
docker compose run --rm php /bin/sh
```
and then - 

```bash
chown -R laravel:laravel /var/www/html
```