---
layout: default
title: "caffeinate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="caffeinate">
  <a href="/zh/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 防止 Mac 进入休眠模式.

#### 防止进入休眠模式 , 1 小时内 (3600 秒）:
```shell
caffeinate -u -t {{3600}}
```
#### 在指定命令执行完前，禁止进入休眠:
```shell
caffeinate -s {{命令}}
```
#### 在你按 Ctrl-C 之前禁止进入休眠模式:
```shell
caffeinate -i
```
{% endraw %}