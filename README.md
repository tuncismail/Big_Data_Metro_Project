# Project README  

## Data Download  
Download the required data from the following link:  
[**Data Download Link**](https://data.ibb.gov.tr/dataset/hourly-public-transport-data-set)  

## Training and Merged Data  
[**Training and Merged Data Link**](https://www.kaggle.com/datasets/alihanyaln/istanbul-public-transportation-dataset)  

---

## How to Start Kafka  

### In Linux  
Start Zookeeper:
 ```bash
/path/to/kafka/bin/zookeeper-server-start.sh /path/to/kafka/config/zookeeper.properties  
```
Start Kafka server:  
```bash
/path/to/kafka/bin/kafka-server-start.sh /path/to/kafka/config/server.properties  
```

### In WSL  
Start Zookeeper:  
 ```bash
  /path/to/kafka/bin/zookeeper-server-start.sh /path/to/kafka/config/zookeeper.properties 
   ```
Start Kafka server:  
```bash
/path/to/kafka/bin/kafka-server-start.sh /path/to/kafka/config/server.properties   
```
---

## Kafka Consumer Code Execution  

Run the Kafka consumer code:  
```bash
consumer_and_load_to_hbase.ipynb  
```
---

## Kafka Producer Code Execution  

Run the Kafka producer code:  
```bash
producer.ipynb  
```
---

## Data format, training, validation: 

  
Model weight is in [checkpoints](https://github.com/tuncismail/Big_data_metro_project/tree/main/checkpoints) folder
```
data_format_and_training.ipynb  
```
---


