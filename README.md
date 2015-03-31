# Alpine Nginx

Tiny web server using nginx built from source on Alpine Linux.

The current version of Nginx availble in apk is 1.6.2:

```sh
/ # apk --update search nginx
nginx-1.6.2-r1
```

This image builds the latest version (1.7.11) from source:

```sh
docker run -it --rm connexiolabs/alpine-nginx:1.7.11 sh

> nginx -v
nginx version: nginx/1.7.11
```

Built image currently weighs in at 28.1 MB:

```sh
❯ docker images | grep connexiolabs/alpine-nginx
connexiolabs/alpine-nginx                     latest              4cbcc8520cc0        2 minutes ago       28.1 MB
connexiolabs/alpine-nginx                     1.7.11              1ae08c4d8414        16 minutes ago      28.1 MB
```
