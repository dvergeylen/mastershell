---
layout: default
title: "aws kinesis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-kinesis">
  <a href="/en/common/aws-kinesis.html">aws kinesis</a> <a href="#aws-kinesis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Official AWS CLI for Amazon Kinesis streaming data services.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/kinesis/index.html#cli-aws-kinesis>.

#### Show all streams in the account:
```shell
aws kinesis list-streams
```
#### Write one record to a Kinesis stream:
```shell
aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data {{base64_encoded_message}}
```
#### Write a record to a Kinesis stream with inline base64 encoding:
```shell
aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data "$( echo "{{my raw message}}" | base64 )"
```
#### List the shards available on a stream:
```shell
aws kinesis list-shards --stream-name {{name}}
```
#### Get a shard iterator for reading from the oldest message in a stream's shard:
```shell
aws kinesis get-shard-iterator --shard-iterator-type TRIM_HORIZON --stream-name {{name}} --shard-id {{id}}
```
#### Read records from a shard, using a shard iterator:
```shell
aws kinesis get-records --shard-iterator {{iterator}}
```
{% endraw %}