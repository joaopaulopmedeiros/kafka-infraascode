# Kafka Cluster

Provisioning infrastructure
```
docker-compose up
```

Listing containers
```
docker-compose ps
```

Accessing container bash terminal
```
docker exec -it cluster-kafka-1-1 bash
```

Creating a topic
```
kafka-topics --create --bootstrap-server localhost:29092 --replication-factor 3 --parti
tions 3 --topic meu-topico
```

Listing a topic
```
kafka-topics --list --bootstrap-server localhost:29092
```

Producing messages
```
kafka-console-producer --broker-list localhost:29092 --topic meu-topico
```

Consuming messages
```
kafka-console-consumer --bootstrap-server localhost:29092 --topic meu-topico
```
