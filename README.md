# nginx-balancer
This is a balancer based on [nginx](https://hub.docker.com/_/nginx/)

## Why

It's a good way to dispatch requests to services. So a dispatcher(or balancer?) is needed.
I searched in the [hub.docker.com](http://hub.docker.com), but the repository [nginx-balancer](https://hub.docker.com/r/strm/nginx-balancer/) has been invalid, so I make it.

## How to use

```
docker build --rm -t your-image-name .
docker run -d -p 80:80 --name your-container-name -v /path/to/logs:/etc/nginx/logs/ your-image-name
```