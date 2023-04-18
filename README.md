# Chat Application
A real-time chat application built with a ReactJS Frontend and Java Spring Boot Backend. Apache Kafka is used as the message broker.




## Before Running the Project 

*Start Zookeeper*
```
[for windows:]
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

zookeeper-server-start .\config\zookeeper.properties
```

*Start Kafka*
```
[for windows:]
.\bin\windows\kafka-server-start.bat .\config\server.properties

kafka-server-start .\config\server.properties
```

*Create a Topic*
```
[for windows:]
.\bin\windows\kafka-topics.bat --create --topic kafka-chat --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1

kafka-topics --create --topic kafka-chat --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1

```

*Start Backend*
```
mvn spring-boot:run
```

*Start Frontend*
```
npm start
```



