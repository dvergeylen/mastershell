---
layout: default
title: "mongod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mongod">
  <a href="/zh/common/mongod.html">mongod</a> <a href="#mongod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MongoDB 数据库服务器。
> 更多信息见：<https://docs.mongodb.com/manual/reference/program/mongod>.

#### 指定配置文件：
```shell
mongod --config {{filename}}
```
#### 指定要监听的端口：
```shell
mongod --port {{port}}
```
#### 指定数据库分析级别，用于性能调优分析。 0 - 关闭，1 - 仅是记录慢速操作，2 - 全部：
```shell
mongod --profile {{0|1|2}}
```
{% endraw %}