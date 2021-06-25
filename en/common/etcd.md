---
layout: default
title: "etcd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="etcd">
  <a href="/en/common/etcd.html">etcd</a> <a href="#etcd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A distributed, reliable key-value store for the most critical data of a distributed system.
> More information: <https://etcd.io>.

#### Start a single-node etcd cluster:
```shell
etcd
```
#### Start a single-node etcd cluster, listening for client requests on a custom URL:
```shell
etcd --advertise-client-urls {{http://127.0.0.1:1234}} --listen-client-urls {{http://127.0.0.1:1234}}
```
#### Start a single-node etcd cluster with a custom name:
```shell
etcd --name {{my_etcd_cluster}}
```
#### Start a single-node etcd cluster with extensive metrics available at http://localhost:2379/debug/pprof/:
```shell
etcd --enable-pprof --metrics extensive
```
{% endraw %}