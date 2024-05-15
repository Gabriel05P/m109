# M109

## Build
docker build -t gpervorfi/m109:latest . --push

## Temporary Run
docker run -p 8080:80 --rm gpervorfi/m109:latest

## Temporary Detached
docker run -p 8080:80 -d gpervorfi/m109:latest