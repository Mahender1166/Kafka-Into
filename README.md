# Kafka-Into
## Kafka Commands:
All commands are executed in powershell as administration permission.
- To start a zookeeper server in a new powershell window ``` bin/zookeeper-server-start.sh config/zookeeper.properties```
- To start a kafka server in a new powershell window ```bin/kafka-server-start.sh config/server.properties```
- To create a topic we use the command ```bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic test``` where test is the sample topic name.
- To view the list of topics present ```bin/kafka-topics.sh --list --bootstrap-server localhost:9092```
- To run as producer for the topic test in new powershell window ```bin/kafka-console-producer.sh --bootstrap-server localhost:9092 --topic test```, where ```test``` is the topic name
- To run as customer for the topic test in new powershell window run the command ```bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning```, where ```test``` is the topic name.

## My commands:
Each command below is executed in new powershell window.
- To run zookeeper server ``` bin/zookeeper-server-start.sh config/zookeeper.properties```
- To run kafka server ```bin/kafka-server-start.sh config/server.properties```
- To create a topic ```bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic laptops```
- To view list of topics ```bin/kafka-topics.sh --list --bootstrap-server localhost:9092```
- To run as producer in laptops ```bin/kafka-console-producer.sh --bootstrap-server localhost:9092 --topic laptops```
- To run  as customer in topic laptops ```bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic laptops --from-beginning```
