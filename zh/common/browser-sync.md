---
layout: default
title: "browser-sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="browser-sync">
  <a href="/zh/common/browser-sync.html">browser-sync</a> <a href="#browser-sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 启动一个本地的服务，可以监听文件改动，刷新浏览器.
> 更多信息: <https://browsersync.io/docs/command-line>.

#### 将指定目录发成服务:
```shell
browser-sync start --server {{路径/到/目录}} --files {{路径/到/目录}}
```
#### 启动当前目录服务，同时监听指定目录下css文件的变动
```shell
browser-sync start --server --files '{{路径/到/目录/*.css}}'
```
#### 创建配置文件:
```shell
browser-sync init
```
#### 按指定配置文件中的配置启动服务:
```shell
browser-sync start --config {{配置文件}}
```
{% endraw %}