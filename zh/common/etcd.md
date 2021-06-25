---
layout: default
title: "etcd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="etcd">
  <a href="/zh/common/etcd.html">etcd</a> <a href="#etcd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 分布式，可靠的键值存储，用于分布式系统中存储最关键的数据。
> 更多信息见：<https://etcd.io>.

#### 启动单节点 etcd 集群：
```shell
etcd
```
#### 启动一个单节点 etcd 集群，在自定义 URL 上侦听客户端请求：
```shell
etcd --advertise-client-urls {{http://127.0.0.1:1234}} --listen-client-urls {{http://127.0.0.1:1234}}
```
#### 使用自定义名称启动单节点 etcd 集群：
```shell
etcd --name {{my_etcd_cluster}}
```
#### 启动单节点 etcd 集群，同时可以在这里看到大量监控指标 http://localhost:2379/debug/pprof/:
```shell
etcd --enable-pprof --metrics extensive
```
{% endraw %}