# Media_Server
Based on
https://www.linuxserver.io/2017/06/24/the-perfect-media-server-2017/
https://github.com/plexinc/pms-docker

## Requires

docker
docker-compose

1. Add user for containers
```shell
useradd dockeruser
id dockeruser
```

2. Create a file /etc/environment
```shell
PUID=1001
PGID=1001
```

3. Create docker compose YML

4. Run docker with docker compose
```shell
# execute docker compose file
docker-compose -f media_server.yml up -d
# get logs from containers
docker-compose -f media_server.yml logs
```
