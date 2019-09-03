# Getting Started with Redis Streams & Java

This project shows how to use [Lettuce Java client](https://lettuce.io) to publish and consume messages using consumer groups.

This is a first basic example that use a single consumer.

### Build

```
> cd redis-streams-101-java

> mvn clean verify

```

### Run

Run the producer

```
> cd redis-streams-101-java

> mvn exec:java -Dexec.mainClass="com.kanibl.redis.streams.simple.RedisStreams101Producer" -Dexec.args="5"
```

Run the consumer

```
> cd redis-streams-101-java

> mvn exec:java -Dexec.mainClass="com.kanibl.redis.streams.simple.RedisStreams101Consumer"
```