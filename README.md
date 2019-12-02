# SF Crime Statistics with Spark Streaming Project

## Introduction 

The aim of the project is to create an Streaming application with Spark that connects to a 
Kafka cluster, reads and process the data.

## Requirements

* Java 1.8.x
* Scala 2.11.x
* Spark 2.4.x
* Kafka
* Python 3.6 or above

## How to use the application

In order to run the application you will need to start:

1. Zookeeper:

`/usr/bin/zookeeper-server-start config/zookeeper.properties`

2. Kafka server:

`/usr/bin kafka-server-start config/properties`

3. Kafka consumer:

`kafka-console-consumer --topic "topic-name" --from-beginning --bootstrap-server localhost:9092`