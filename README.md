# kafka-from-wikimedia
Microservices exchanging data from wikimdia https://stream.wikimedia.org/v2/stream/recentchange

This is a project composed by two microservices that comunicate with each other assyncronowsly using Apache Fafka.
The Producer microservice reads the data from https://stream.wikimedia.org/v2/stream/recentchange and drops it in the Kafka.
The Consumer reads from the queue and stores in the MySQL database.
