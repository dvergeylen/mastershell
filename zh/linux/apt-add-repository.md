---
layout: default
title: "apt-add-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-add-repository">
  <a href="/zh/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 apt 仓库。

#### 添加一个 apt 仓库：
```shell
apt-add-repository {{repository_spec}}
```
#### 移除一个 apt 仓库：
```shell
apt-add-repository --remove {{repository_spec}}
```
#### 添加一个 apt 仓库之后更新包缓存：
```shell
apt-add-repository --update {{repository_spec}}
```
#### 开启源码包：
```shell
apt-add-repository --enable-source {{repository_spec}}
```
{% endraw %}