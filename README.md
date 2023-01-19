# kafka-from-wikimedia
Microservices exchanging data from wikimdia https://stream.wikimedia.org/v2/stream/recentchange

This is a Spring Boot project composed by two microservices that comunicate with each other assyncronously using Apache Kafka exchanging a large amount of data.
The Producer microservice reads the data from https://stream.wikimedia.org/v2/stream/recentchange and drops it in the Kafka.
The Consumer reads from the queue and stores in the MySQL database.
