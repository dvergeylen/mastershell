---
layout: default
title: "choco feature"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-feature">
  <a href="/ja/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolateyで機能を操作します.
> 詳しくはこちら: <https://chocolatey.org/docs/commands-feature>.

#### 利用可能な機能のリストを表示します:
```shell
choco feature list
```
#### 機能を有効にします:
```shell
choco feature enable --name {{名}}
```
#### 機能を無効にします:
```shell
choco feature disable --name {{名}}
```
{% endraw %}