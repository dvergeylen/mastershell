---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/zh/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache 基准测试工具.最简单的压力测试工具.

#### 向目标 URL 执行 100 次 HTTP GET 请求:
```shell
ab -n {{100}} {{url}}
```
#### 使用 10 个并发请求，同时向目标 URL 执行 100 次 HTTP GET 请求:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### 使用 keep alive:
```shell
ab -k {{url}}
```
#### 为基准测试设置最大的测试时间（单位：秒）:
```shell
ab -t {{60}} {{url}}
```
{% endraw %}