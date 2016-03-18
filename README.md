# kafka-statsd

Send your Kafka offset lags to StatsD.

## Usage

```
kafka-statsd --zookeeper --zookeeper-addrs host1:2181,host2:2181 --statsd-addr=statsd:8125 --prefix kafka.
```

## Install

```
$ go get github.com/travisjeffery/kafka-statsd
```

## License

MIT

---

- [travisjeffery.com](http://travisjeffery.com) 
- Twitter [@travisjeffery](https://twitter.com/travisjeffery)
- GitHub [@travisjeffery](https://github.com/travisjeffery) 
