---
layout: default
title: "etcdctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="etcdctl">
  <a href="/en/common/etcdctl.html">etcdctl</a> <a href="#etcdctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI interface for interacting with etcd, a highly-available key-value pair store.
> More information: <https://etcd.io/docs/latest/dev-guide/interacting_v3/>.

#### Display the value associated with a specified key:
```shell
etcdctl get {{my/key}}
```
#### Store a key-value pair:
```shell
etcdctl put {{my/key}} {{my_value}}
```
#### Delete a key-value pair:
```shell
etcdctl del {{my/key}}
```
#### Store a key-value pair, reading the value from a file:
```shell
etcdctl put {{my/file}} < {{path/to/file.txt}}
```
#### Save a snapshot of the etcd keystore:
```shell
etcdctl snapshot save {{path/to/snapshot.db}}
```
#### Restore a snapshot of an etcd keystore (restart the etcd server afterwards):
```shell
etcdctl snapshot restore {{path/to/snapshot.db}}
```
#### Add a user:
```shell
etcdctl user add {{my_user}}
```
#### Watch a key for changes:
```shell
etcdctl watch {{my/key}}
```
{% endraw %}