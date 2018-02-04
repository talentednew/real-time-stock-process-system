# Code of Redis Part

## redis-producer.py
Redis producer, fetch the message from Kafka topic and publish to redis PUB

### Code Dependence
kafka-python    https://github.com/dpkp/kafka-python
redis           https://pypi.python.org/pypi/redis

```sh
pip install -r requirements.txt
```

### 运行代码
If the kafka and redis are running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101
```sh
python redis-publisher.py average-stock-price 192.168.99.101:9092 average-stock-price 192.168.99.101 6379
```


