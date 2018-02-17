# Media_Server
Based on
https://www.linuxserver.io/2017/06/24/the-perfect-media-server-2017/
https://github.com/plexinc/pms-docker
https://hub.docker.com/u/linuxserver/

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

## Testing
`sudo nano /etc/hosts`

```shell
# Local Test Media Server
127.0.0.1   radarr.docker.local
127.0.0.1   sonar.docker.local
127.0.0.1   transmission-sonarr.docker.local
127.0.0.1   transmission-radarr.docker.local
127.0.0.1   jackett.docker.local
```
