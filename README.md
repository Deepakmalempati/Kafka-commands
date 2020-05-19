# commands used for Kafka

1. To run Zookeeper service  
```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties```
1. To run kafka service  
```.\bin\windows\kafka-server-start.bat .\config\server.properties```
1. command to create topic  
```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic hello-language-messages```
1. Command used to view list of topics  
```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list```
1. To run Kafka producer  
```.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic hello-language-messages```
1. To run kafka consumer  
```.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic hello-language-messages --from-beginning```
