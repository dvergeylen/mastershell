---
layout: default
title: "pwgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pwgen">
  <a href="/zh/osx/pwgen.html">pwgen</a> <a href="#pwgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 生成可拼写发音的密码.

#### 生成指定长度的随机密码:
```shell
pwgen -y {{长度}}
```
#### 生成安全、难以记忆的密码:
```shell
pwgen -s {{长度}}
```
#### 生成至少包含一个大写字母的密码:
```shell
pwgen -c {{长度}}
```
{% endraw %}