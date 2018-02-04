# The Code of Cassandra Part

## data-storage.py
the implementation of a Cassandra storage process

### Code Dependence
cassandra-driver    https://github.com/datastax/python-driver

cql

```sh
pip install -r requirements.txt
```

### Running Process
If the cassandra is running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101

Apply cqlsh client to create a keyspace and table
```sh
CREATE KEYSPACE "stock" WITH replication = {'class': 'SimpleStrategy', 'replication_factor': 1} AND durable_writes = 'true';
USE stock;
CREATE TABLE stock (stock_symbol text, trade_time timestamp, trade_price float, PRIMARY KEY (stock_symbol,trade_time));
```

```sh
python data-storage.py stock-analyzer 192.168.99.101:9092 stock stock 192.168.99.101
```
