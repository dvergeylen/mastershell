---
layout: default
title: "sqsc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sqsc">
  <a href="/en/common/sqsc.html">sqsc</a> <a href="#sqsc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line AWS Simple Queue Service client.
> More information: <https://github.com/yongfei25/sqsc>.

#### List all queues:
```shell
sqsc lq {{queue_prefix}}
```
#### List all messages in a queue:
```shell
sqsc ls {{queue_name}}
```
#### Copy all messages from one queue to another:
```shell
sqsc cp {{source_queue}} {{destination_queue}}
```
#### Move all messages from one queue to another:
```shell
sqsc mv {{source_queue}} {{destination_queue}}
```
#### Describe a queue:
```shell
sqsc describe {{queue_name}}
```
#### Query a queue with SQL syntax:
```shell
sqsc query "SELECT body FROM {{queue_name}} WHERE body LIKE '%user%'"
```
#### Pull all messages from a queue into a local sqlite database in your present working directory:
```shell
sqsc pull {{queue_name}}
```
{% endraw %}