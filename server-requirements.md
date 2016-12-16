At least 1GB Memory

Mysql (or remote if not installed on the same host)
Git
Docker
Docker Compose

// To download docker compose
https://github.com/docker/compose/releases
```
$ sudo chown -R $(whoami) /usr/local/bin
```

To run docker-compose up , might need to use sudo or add myself to group
``` 
$ usermod -aG docker ${USER}
```