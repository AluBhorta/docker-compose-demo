# Docker Compose Demo

This repo is used as a demo for [this blog](https://techmormo.com/posts/what-is-docker-compose/).
## Prerequisites

- [Docker](https://docs.docker.com/engine/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Usage

start the app in the background

```sh
docker compose up -d
```

check the logs (use `-f` to follow)

```sh
docker compose logs
```

remove the app

```sh
docker compose down
```

rebuild images (after making changes)

```sh
docker compose build
```

update web service (eg. with new image)

```sh
docker compose up web -d --no-deps
```

## Notes

- the `master` branch contains the code for flask dev server (`flask run`).
- the `prod` branch contains the code for `gunicorn`.

## Acnkowledgement

This demo was adapted from docker compose [getting started](https://docs.docker.com/compose/gettingstarted/) guide.
