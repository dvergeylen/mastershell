---
layout: default
title: "logstash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logstash">
  <a href="/en/common/logstash.html">logstash</a> <a href="#logstash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An Elasticsearch ETL (extract, transform and load) tool.
> Commonly used to load data from various sources (such as databases and log files) into Elasticsearch.
> More information: <https://www.elastic.co/products/logstash>.

#### Check validity of a logstash configuration:
```shell
logstash --configtest --config {{logstash_config.conf}}
```
#### Run logstash using configuration:
```shell
sudo logstash --config {{logstash_config.conf}}
```
#### Run logstash with the most basic inline configuration string:
```shell
sudo logstash -e 'input {} filter {} output {}'
```
{% endraw %}