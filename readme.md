# Docker + Compose + Swarm + Traefik

### how to use?

Clone this repo

```
git clone https://github.com/almirtoledo/docker-swarm
```

Create your cluster

```
docker swarm init --advertise-addr YOUR_IP
```

Create your network for swarm cluster

```
docker network create --driver overlay YOUR_NETWORK_NAME
```

Traefik deploy:

```
docker stack deploy --compose-file traefik.yml traefik
```

Services exemple deploy:

```
docker stack deploy --compose-file services.yml services
```

### Autor

- Almir Toledo [@almirtoledo](https://www.github.com/almirtoledo)
