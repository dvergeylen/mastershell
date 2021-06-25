---
layout: default
title: "consul-kv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="consul-kv">
  <a href="/en/common/consul-kv.html">consul-kv</a> <a href="#consul-kv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Distributed key-value store with health checking and service discovery.
> More information: <https://learn.hashicorp.com/consul/getting-started/kv>.

#### Read a value from the key-value store:
```shell
consul kv get {{key}}
```
#### Store a new key-value pair:
```shell
consul kv put {{key}} {{value}}
```
#### Delete a key-value pair:
```shell
consul kv delete {{key}}
```
{% endraw %}