# Traefik Coraza plugin debugging test with HTTPS

## Start containers

```sh
docker compose up
```

## Test GET

```sh
curl -k -vvv -L https://whoami.localhost/
```

## Test /admin

```sh
curl -k -vvv -L https://whoami.localhost/admin
```

## Test POST

```sh
curl -k -vvv -L --request POST \
  --url https://whoami.localhost/ \
  --header 'Content-Type: application/x-www-form-urlencoded' \
  --data key=value
```
