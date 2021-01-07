# Private Docker Registry

Easy create a new private docker registry. In this instance it sits behind `traefik` reverse proxy.

# Adding password

add a new dir call `/auth`

```
mkdir auth
```

generate a new username and password and place it inside the `/auth`

```
htpasswd -Bbn user password > auth/htpasswd
```

# Run docker compose

```
docker-compose up -d
```
