### [YoPass](https://github.com/jhaals/yopass) with [Redis](https://github.com/redis/redis), which includes YoPass's monitoring using [Prometheus](https://github.com/prometheus/prometheus) and [Grafana](https://github.com/grafana/grafana)

1. Requires [docker](https://docs.docker.com/get-docker/) and [compose](https://docs.docker.com/compose/install/)
2. Parameterized using variables in the [`.env`](.env) file
3. Up the project using command:
```
docker compose up -d
```

| App | Port | Username | Password
|-|-|-|-
| YoPass | 1337 | | 
| Prometheus | 9090 | |
| Grafana | 3000 | `admin` | `admin`

| Useful commands | Description
|-|-
| `docker stats` | Containers resource usage (`--no-stream` only pull the first result)
| `docker compose logs` | Shows logs of containers (`-f` to follow logs)
| `docker compose down` | Stop and remove containers (`-v` remove named volumes declared in the volumes section of the Compose file and anonymous volumes attached to containers)
| `docker system prune -a -f` | Remove all unused containers, networks, images (`--volumes` prune volumes)
