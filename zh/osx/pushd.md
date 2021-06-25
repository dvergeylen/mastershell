---
layout: default
title: "pushd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pushd">
  <a href="/zh/osx/pushd.html">pushd</a> <a href="#pushd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将目录放在堆栈上，以便以后访问.
> 另请参阅 `popd` 命令说明，以切换回原始目录.

#### 切换到目录并将其添加到堆栈上:
```shell
pushd {{directory}}
```
#### 切换堆栈上的第一个和第二个目录:
```shell
pushd
```
#### 通过使第 5 个元素成为堆栈的顶部来旋转堆栈:
```shell
pushd +4
```
{% endraw %}