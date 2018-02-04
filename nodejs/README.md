# Code of Node.js related Part

## index.js
实现了一个简单的前端应用实时显示数据动态
Implementation of one simple real time UI to visualize the the stock data

### Code Dependence
socket.io       http://socket.io/
redis           https://www.npmjs.com/package/redis
smoothie        https://www.npmjs.com/package/smoothie
minimist        https://www.npmjs.com/package/minimist

```sh
npm install
```

### Running Process
If all the services are running in one docker machine called stockData, the ip of virtual machine is 192.168.99.101
```sh
node index.js --port=3000 --redis_host=192.168.99.101 --redis_port=6379 --subscribe_topic=average-stock-price
```
