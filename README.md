# FLiP-CDC
Using Debezium CDC Connectors (Postgresql, Mysql, MongoDB) with Apache Pulsar


#### Debezium Connectors
 
* https://debezium.io/blog/2019/05/23/tutorial-using-debezium-connectors-with-apache-pulsar/
 
#### Mysql, postgrsql, mongodb -> Debezium -> cdc to pulsar -> function -> sinks and display

 
#### NiFi feed -> Mongo -> Pulsar CDC

* https://hub.streamnative.io/connectors/debezium-postgres-source/2.5.1/
* https://hub.streamnative.io/connectors/debezium-mysql-source/2.5.1/
* https://pulsar.apache.org/docs/en/io-cdc-debezium/
* https://hub.streamnative.io/connectors/debezium-mongodb-source/2.5.1/
* https://github.com/debezium/debezium-examples/blob/main/apache-pulsar/README.md

### Data Ideas

* weather
* stocks
* sensors
* logs
* https://urlscan.io/docs/api/#search
* https://docs.abuseipdb.com/#introduction
* https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_hour.atom
* https://pulsar.apache.org/docs/en/io-cdc-debezium/


### MongoDB, Postgresql, MySQL

* https://github.com/apache/pulsar/blob/master/pulsar-io/debezium/mongodb/src/main/resources/debezium-mongodb-source-config.yaml


### Example docker setup

* https://hub.docker.com/r/debezium/server
* https://hub.docker.com/_/mongo

````
# 8080
docker run -it --name debezium -p 9999:9999 -v $PWD/conf:/debezium/conf -v $PWD/data:/debezium/data debezium/server



````
