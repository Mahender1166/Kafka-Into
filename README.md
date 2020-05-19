# Kafka-Into
## Kafka Commands:
All commands are executed in powershell as administration permission.
- To start a zookeeper server in a new powershell window ```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties```
- To start a kafka server in a new powershell window ```.\bin\windows\kafka-server-start.bat .\config\server.properties```
- To create a topic we use the command ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic test``` where test is the sample topic name.
- To view the list of topics present ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list```
- To run as producer for the topic test in new powershell window ```.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic test```, where ```test``` is the topic name
- To run as customer for the topic test in new powershell window run the command ```.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic test --from-beginning```, where ```test``` is the topic name.

## My commands:
Each command below is executed in new powershell window.
- To run zookeeper server ```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties```
- To run kafka server ```.\bin\windows\kafka-server-start.bat .\config\server.properties```
- To create a topic ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic laptops```
- To view list of topics ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list```
- To run as producer in laptops ```.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic laptops```
- To run  as customer in topic laptops ```.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic laptops --from-beginning```
