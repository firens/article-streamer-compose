Compose file for server deployment of [article-streamer](https://github.com/firens/article-streamer) project

# Configuration
 
 In order to run this project you need to provide Twitter and Mysql configurations.
 You wil need a twitter application account and an instance of Mysql v5.7 (tested with 5.7.16)

 Create a file *docker-env.list* containing the following keys and fill the values
 
 ```
# Twitter authentication keys
TW_CONS_KEY=
TW_CONS_SEC=
TW_ACC_TOKEN=
TW_ACC_SEC=

# Mysql host
MYSQL_HOST=
MYSQL_JDBC_URL=
MYSQL_USER=
MYSQL_PSWD=
```

# Start the system

Simply run docker compose

``` 
$ docker-compose up -d
```

To check the logs of each of the elements
```
$ docker-compose logs [aggregator/score_updater/processor/webapp/data_server]
```