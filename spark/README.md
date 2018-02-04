# Code of Spark Part

## stream-process.py

### Code Dependence
pyspark         http://spark.apache.org/docs/latest/api/python/
kafka-python    https://github.com/dpkp/kafka-python


### Running Process
If the kafka is running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101
```sh
```sh
spark-submit --jars spark-streaming-kafka-0-8-assembly_2.11-2.0.0.jar stream-processing.py stock-analyzer average-stock-price 192.168.99.101:9092
```