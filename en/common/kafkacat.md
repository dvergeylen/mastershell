---
layout: default
title: "kafkacat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kafkacat">
  <a href="/en/common/kafkacat.html">kafkacat</a> <a href="#kafkacat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache Kafka producer and consumer tool.
> More information: <https://github.com/edenhill/kafkacat>.

#### Consume messages starting with the newest offset:
```shell
kafkacat -C -t {{topic}} -b {{brokers}}
```
#### Consume messages starting with the oldest offset and exit after the last message is received:
```shell
kafkacat -C -t {{topic}} -b {{brokers}} -o beginning -e
```
#### Consume messages as a Kafka consumer group:
```shell
kafkacat -G {{group_id}} {{topic}} -b {{brokers}}
```
#### Publish message by reading from stdin:
```shell
 echo {{message}} | kafkacat -P -t {{topic}} -b {{brokers}}
```
#### Publish messages by reading from a file:
```shell
kafkacat -P -t {{topic}} -b {{brokers}} {{path/to/file}}
```
#### List metadata for all topics and brokers:
```shell
kafkacat -L -b {{brokers}}
```
#### List metadata for a specific topic:
```shell
kafkacat -L -t {{topic}} -b {{brokers}}
```
#### Get offset for a topic/partition for a specific point in time:
```shell
kafkacat -Q -t {{topic}}:{{partition}}:{{unix_timestamp}} -b {{brokers}}
```
{% endraw %}