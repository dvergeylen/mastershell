---
layout: default
title: "aws kinesis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-kinesis">
  <a href="/de/common/aws-kinesis.html">aws kinesis</a> <a href="#aws-kinesis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Offizielles AWS CLI für die Amazon Kinesis-Streaming-Datenplattform.
> Weitere Informationen: <https://docs.aws.amazon.com/cli/latest/reference/kinesis/index.html#cli-aws-kinesis>.

#### Liste alle Streams auf:
```shell
aws kinesis list-streams
```
#### Schreibe einen Datensatz in einen Kinesis Stream:
```shell
aws kinesis put-record --stream-name {{name}} --partition-key {{schlüssel}} --data {{base64_codierte_nachricht}}
```
#### Schreibe einen Datensatze in einen Kinesis Stream mit base64 inline Encodierung:
```shell
aws kinesis put-record --stream-name {{name}} --partition-key {{schlüssel}} --data "$( echo "{{meine nachricht}}" | base64 )"
```
#### Liste alle verfügbaren Shards in einem Stream auf:
```shell
aws kinesis list-shards --stream-name {{name}}
```
#### Rufe einen Shard Iterators auf, um diesen beginnend mit der ältesten Nachricht auszulesen:
```shell
aws kinesis get-shard-iterator --shard-iterator-type TRIM_HORIZON --stream-name {{name}} --shard-id {{id}}
```
#### Lies einen Datensatz aus einem Shard über einen Shard Iterator:
```shell
aws kinesis get-records --shard-iterator {{iterator}}
```
{% endraw %}