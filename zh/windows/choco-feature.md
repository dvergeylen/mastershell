---
layout: default
title: "choco feature"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-feature">
  <a href="/zh/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolatey 的交互功能.

#### 显示可用的功能列表:
```shell
choco feature list
```
#### 启用一个功能:
```shell
choco feature enable --name {{功能名称}}
```
#### 禁用一个功能:
```shell
choco feature disable --name {{功能名称}}
```
{% endraw %}