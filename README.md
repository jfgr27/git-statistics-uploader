# GitDataUploader
A service that handles Client GitStats requests, pushing the raw data on an Kafka event queue.

# Table of Contents

# Installation 
## Local Installation
The following steps instruct how to deploy this service locally

## Docker Installation

# Usage





TO DETETE

# Git API
```sh
curl https://api.github.com/users/jamesrea97/repos

```


# Kafka notes
Kafka Setup up locally

```sh
# Downlaod lates version of Kakfa. (Currently: kafka_2.13-2.8.0)
curl https://downloads.apache.org/kafka/2.8.0/kafka_2.13-2.8.0.tgz --output kafka_2.13-2.8.0.tgz 
# Extract zipped file
tar -xzf kafka_2.13-2.8.0.tgz
# cd into kakfka
cd kafka_2.13-2.8.0
# Starts necessary Zookeeper - used for resource management in Kafka
bin/zookeeper-server-start.sh config/zookeeper.properties
# Starts Kafka broker service
bin/kafka-server-start.sh config/server.properties
```

Creating a topic
```sh
bin/kafka-topics.sh --create --topic topic-name --bootstrap-server localhost:9092
```
Check topic status
```
bin/kafka-topics.sh --describe --topic topic-name--bootstrap-server localhost:9092
```