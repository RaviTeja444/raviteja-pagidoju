# raviteja-pagidoju
# Install Kafka
Added Changes
Download the Kafka and install it to C: drive

The $ indicates a Bash prompt.

```$ tar -xzf kafka_2.13-2.7.0.tgz```

```$ cd kafka_2.13-2.7.0```

# Kafka Setting
## Following are the commands to be executed

ZooKeeper service....

$ bin/zookeeper-server-start.sh config/zookeeper.properties

Kafka service...

$ bin/kafka-server-start.sh config/server.properties

topic creation...

.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic ravi-message
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list

Kafka Producer 

.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic ravi-message

 Kafka Consumer

.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic ravi-message --from-beginning
