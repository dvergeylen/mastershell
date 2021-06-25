---
layout: default
title: "shuf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shuf">
  <a href="/zh/osx/shuf.html">shuf</a> <a href="#shuf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 生成随机排列.

#### 随机化文件中的行顺序并输出结果:
```shell
shuf {{文件名}}
```
#### 只输出结果的前 5 条:
```shell
shuf -n {{5}} {{文件名}}
```
#### 将结果输出写入另一个文件:
```shell
shuf {{文件名}} -o {{输出_文件名}}
```
#### 生成范围 (1-10) 内的随机数:
```shell
shuf -i {{1-10}}
```
{% endraw %}