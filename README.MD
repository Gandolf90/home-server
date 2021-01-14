# Install

  - first install Docker for your system : https://docs.docker.com/get-docker/
  - install "docker-compose" ( linux & mac )

# 1. Copy .env.example to .env:
```sh
$ cp .env.example .env
```
# 2. fill information for your environment

```sh
MYSQL_ROOT_PASSWORD=SUPERSECRETPASSWORD
MYSQL_DATABASE=nextcloud
MYSQL_USER=user
MYSQL_PASSWORD=password
MYSQL_HOST=db
DOMAIN=test.de
DOMAIN_EMAIL=test@test.de
VIRTUAL_PORT=80
VIRTUAL_NETWORK=nginx-proxy
```

# 3. Fire it up!

```sh
$ docker-compose up
```

if you want to launch it in the backgroud use "-d"

```sh
$ docker-compose up -d
```

LOCAL LINKS:

1. adminer (web-mysql-client): http://{ip-of-your-system}:8181/
2. portainer (web-docker-manage-tool): http://{ip-of-your-system}:9001/
3. nextcloud: http://{domain-you-configured-in-environment}/
or https://{domain-you-configured-in-environment}/

# have fun!