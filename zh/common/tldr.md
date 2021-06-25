---
layout: default
title: "tldr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr">
  <a href="/zh/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 简化过的 man 帮助手册.
> 更多信息：<https://tldr.sh>.

#### 获取一个命令的用例 （提示：这就是你怎么得到本信息的）:
```shell
tldr {{command}}
```
#### 展示 Linux 下 tar 的 tldr 文档:
```shell
tldr -p {{linux}} {{tar}}
```
#### 获取一个 Git 子命令的帮助:
```shell
tldr {{git checkout}}
```
#### 更新本地页面 (如果客户端支持缓存):
```shell
tldr -u
```
{% endraw %}