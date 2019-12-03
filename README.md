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

`/usr/bin/kafka-server-start config/server.properties`

3. Kafka consumer:

`kafka-console-consumer --topic "topic-name" --from-beginning --bootstrap-server localhost:9092`

4. Run Spark job:

`spark-submit --packages org.apache.spark:spark-sql-kafka-0-10_2.11:2.3.4 --master local[*] data_stream.py`


### Kafka Consumer Console Output

![kafka consumer output](https://github.com/rubengura/SF_Crime_Statistics/blob/master/kafka-consumer-console-output.PNG)

### Progress Reporter

![progress reporter](https://github.com/rubengura/SF_Crime_Statistics/blob/master/progress_report_console_output.PNG)

### Count Output

![count output](https://github.com/rubengura/SF_Crime_Statistics/blob/master/count_console_output.PNG)