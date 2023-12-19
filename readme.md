# Simple Docker LEMP Stack
goes well with [OrbStack](https://orbstack.dev) for local development.

## Sample Setup with OrbStack
Project 1: https://project1.docker.local
```yml
# project1 docker-compose.yml
...
  nginx:
    ...
    labels:
      - dev.orbstack.domains=project1.docker.local
    networks:
      - docker-network # created external network
```

Project 2: https://project2.docker.local
```yml
# project2 docker-compose.yml
...
  nginx:
    ...
    labels:
      - dev.orbstack.domains=project2.docker.local
    networks:
      - docker-network
```
