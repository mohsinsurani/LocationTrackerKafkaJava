# LocationTrackerKafkaJava

Software to install:
Docker
VScode
Maven Installation for the packages
Java 

start zooper:
docker run -p 2181:2181 zookeeper

start kafka:
docker run -p 9092:9092 \
-e KAFKA_ZOOKEEPER_CONNECT=<Use your IP>:2181 \
-e KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://<Use your IP>:9092 \
-e KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR=1 \
confluentinc/cp-kafka

Run main files of the both the projects. Hit the API with 8080 port from postman which will generate location dynamically
