# Pentaho Data Integration x Apache Kafka

How to get stream data from Kafka topic using Pentaho Data Integration (kettle).

Official tutorial: https://help.pentaho.com/Documentation/8.0/Products/Data_Integration/Transformation_Step_Reference/Kafka_Consumer

In this repository, we provides sample working PDI tranformation based on the tutorial. The goal is to parse incoming data, then put the result into different files, error files or success files.

There are 2 transformation files:
1. Sent-Mail-Consumer.ktr<br>
![Alt text](Sent-Mail-Consumer.JPG?raw=true "Sent-Mail-Consumer Transformation")

2. Sent-Email.ktr<br>
![Alt text](Sent-Email.JPG?raw=true "Sent-Email Transformation")
