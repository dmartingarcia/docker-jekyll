# docker-jekyll

It is part of a [set of repositories](https://github.com/search?q=user%3Admartingarcia+docker) that contain dockerised environments for small applications.

In this case, it contains a self-efficient *Jekyll blog* setup.

## How to use it

```
cp .env.example .env
docker-compose up -d
```

And browse into `http://localhost:4000` in order to see the `jekyll` homepage.

## Traefik integration`

It also contains a Traefik integration, that interact with this reverse proxy, routing request to each container in case it matches the specified domain

There's a domains exposed:
  - your.domain.com

## .env setup

It contains a basic set of variables like:

- HTTP host that uses Traefik to match requests

Please take a look on that and configure it to match your domain.

## Docker Traefik

If you want to use this Traefik integration, [take a look at this repository](https://github.com/dmartingarcia/docker-traefik)
