# kafka-statsd

Send your Kafka offset lags to StatsD.

## Usage

```
kafka-statsd --zookeeper-addrs host1:2181,host2:2181 --statsd-addr=statsd:8125 --statsd-prefix kafka.
```

### Args

**--zookeeper-addrs** - List of Zookeeper addresses, comma delimited. Supports Zookeeper chroots for Kafka metadata that do not reside under the root node, e.g. `host1:2181,host2:2181/kafka`.

**--statsd-address** - StatsD address.

**--statsd-prefix** - StatsD prefix.

**--refresh-interval** - Interval to refresh offset lag, in seconds. Default is 5s.

## Install

Go get:

```
$ go get github.com/travisjeffery/kafka-statsd
```

Docker:

```
$ docker run -d travisjeffery/kafka-statsd --zookeeper-addrs host1:2181,host2:2181 --statsd-addr=statsd:8125 --statsd-prefix kafka.
```

## License

MIT

---

- [travisjeffery.com](http://travisjeffery.com)
- Twitter [@travisjeffery](https://twitter.com/travisjeffery)
- GitHub [@travisjeffery](https://github.com/travisjeffery)
