---
layout: default
title: "ranger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ranger">
  <a href="/en/common/ranger.html">ranger</a> <a href="#ranger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Console file manager with VI key bindings.
> More information: <https://github.com/ranger/ranger>.

#### Launch ranger:
```shell
ranger
```
#### Show only directories:
```shell
ranger --show-only-dirs
```
#### Change the configuration directory:
```shell
ranger --confdir={{path/to/directory}}
```
#### Change the data directory:
```shell
ranger --datadir={{path/to/directory}}
```
#### Print CPU usage statistics on exit:
```shell
ranger --profile
```
{% endraw %}