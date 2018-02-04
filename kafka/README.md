# Code of Kafka Part

## Install Dependence
```sh
pip install -r requirements.txt
```

## google-data-producer.py
Implementation fo one kafka producer, fetch the information of one stock with symbol name from Google finance per second, send to Kafka

### Code Dependence
googlefinance   https://pypi.python.org/pypi/googlefinance
kafka-python    https://github.com/dpkp/kafka-python
schedule        https://pypi.python.org/pypi/schedule

### Running Process
If the kafka is running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101
```sh
python google-data-producer.py AAPL stock-analyzer 192.168.99.101:9092
```

## yahoo-data-producer.py
Implementation fo one kafka producer, fetch the information of one stock with symbol name from Yahoo finance per second, send to Kafka

### Code Dependence
yahoofinance   https://pypi.python.org/pypi/yahoo-finance/1.1.4
kafka-python    https://github.com/dpkp/kafka-python
schedule        https://pypi.python.org/pypi/schedule

### Running Process
If the kafka is running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101
```sh
python yahoo-data-producer.py AAPL stock-analyzer 192.168.99.101:9092
```

## tushare-data-producer.py
Implementation fo one kafka producer, fetch the information of one stock with symbol code from tushare per second, send to Kafka (revised the depracation of some functionalities of yahoo finance and google finance)

### Code Dependence
tushare   https://pypi.python.org/pypi/tushare
kafka-python    https://github.com/dpkp/kafka-python
schedule        https://pypi.python.org/pypi/schedule

### Running Process
If the kafka is running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101
```sh
python tushare-data-producer.py AAPL stock-analyzer 192.168.99.101:9092
```
