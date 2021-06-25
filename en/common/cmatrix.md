---
layout: default
title: "cmatrix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmatrix">
  <a href="/en/common/cmatrix.html">cmatrix</a> <a href="#cmatrix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shows a scrolling Matrix like screen in the terminal.
> More information: <https://github.com/abishekvashok/cmatrix>.

#### Enable asynchronous scrolling:
```shell
cmatrix -a
```
#### Display red text:
```shell
cmatrix -C {{red}}
```
#### Enable rainbow mode:
```shell
cmatrix -r
```
#### Set screen update delay to 2 centiseconds (20 milliseconds):
```shell
cmatrix -u {{2}}
```
{% endraw %}