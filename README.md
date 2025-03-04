# Docker node chrome

Docker image with node and chrome headless

Node version : 22.14.0

Chrome version : latest

# Build

```bash
docker buildx create --use --name node-chrome-builder
docker buildx build --push --platform linux/amd64 -t illuin/node-chrome:release-22.14.0 .
docker buildx stop node-chrome-builder
docker buildx rm node-chrome-builder
```
