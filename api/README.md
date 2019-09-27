# Rest API Server

## Development

To run development Docker use docker-compose:

```sh
docker-compose up [--build]
```

Or you can build and run Docker without compose:

```sh
docker build -f Dockerfile.dev -t [domain/]h.api.dev .
docker run [-d] -p 3000:3000 -v $(pwd):/app/ [domain/]h.api.dev
```
