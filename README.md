# Pentaho Data Integration x Apache Kafka

How to get stream data from Kafka topic using Pentaho Data Integration (kettle).

Official tutorial: https://help.pentaho.com/Documentation/8.0/Products/Data_Integration/Transformation_Step_Reference/Kafka_Consumer

This repository provides sample working PDI tranformation based on the tutorial. The goal is to parse incoming streaming data, then put the result into different files, error files or success files.

There are 2 transformation files:
1. Sent-Mail-Consumer.ktr<br>
This is the parent transformation, where details about Kafka is needed, and also the sub-transformation location path.<br>
![Alt text](img/Sent-Mail-Consumer.JPG?raw=true "Sent-Mail-Consumer Transformation") <br>
![Alt text](img/Sent-Mail-Consumer-Details.JPG?raw=true "Detail of Kafka Consumer")

2. Sent-Email.ktr<br>
This is the sub-transfomartion, where the transformation process or data loading happened.<br>
![Alt text](img/Sent-Email.JPG?raw=true "Sent-Email Transformation")
<br>Sub-transformation should start with 'Get records from stream' plugin. Inside the plugin the only thing needs to specify is the message field name.<br>
![Alt text](img/Sent-Email-Stream.JPG?raw=true "Sent-Email Transformation")
