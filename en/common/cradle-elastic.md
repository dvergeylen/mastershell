---
layout: default
title: "cradle elastic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-elastic">
  <a href="/en/common/cradle-elastic.html">cradle elastic</a> <a href="#cradle-elastic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the ElasticSearch instances for a Cradle instance.
> More information: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#elastic>.

#### Truncate the ElasticSearch index:
```shell
cradle elastic flush
```
#### Truncate the ElasticSearch index for a specific package:
```shell
cradle elastic flush {{package_name}}
```
#### Submit the ElasticSearch schema:
```shell
cradle elastic map
```
#### Submit the ElasticSearch schema for a specific package:
```shell
cradle elastic map {{package_name}}
```
#### Populate the ElasticSearch indices for all packages:
```shell
cradle elastic populate
```
#### Populate the ElasticSearch indices for a specific package:
```shell
cradle elastic populate {{package_name}}
```
{% endraw %}