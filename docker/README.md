# Docker Environment Script Settings

## Code Structure

1. local-setup.sh Fast implementation of single node Kakfa, Cassandra, Zookeeper development environment

## MacOS, Linux

1. create a docker-machine cirtual machine, 2 CPU, 2G storage
```sh
docker-machine create --driver virtualbox --virtualbox-cpu-count 2 --virtualbox-memory 2048 stockData
```
2. Run script program to start all the docker containers (Kafka, Cassandra, Zookeeper)
```sh
./local-setup.sh stockData
```

