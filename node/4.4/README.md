# Node

A Windows Docker container with Node.js 4.4.4 installed.

## Building

```
docker build -t node .
docker tag node:latest node:4.4.4
```

## Onbuild

```
docker build -t node:onbuild onbuild
```
