Kafka Meets Docker
===

[ZooKeeper](https://hub.docker.com/_/zookeeper/)

## Host
```
docker run -d --name=sksvr1 --hostname=sksvr1 zookeeper

docker run -ti --link zksvr1:sksvr1 -p 9160:9160 --name=kafkasvr1 --hostname=kafkasvr1 uiarch/kafka
```
## Kafka Container
```
bin/kafak-server-start.sh config/server.properties
```
