---
layout: default
title: "axel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="axel">
  <a href="/en/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download accelerator.
> Supports HTTP, HTTPS, and FTP.
> More information: <https://github.com/axel-download-accelerator/axel>.

#### Download a URL to a file:
```shell
axel {{url}}
```
#### Download and specify filename:
```shell
axel {{url}} -o {{filename}}
```
#### Download with multiple connections:
```shell
axel -n {{connections_num}} {{url}}
```
#### Search for mirrors:
```shell
axel -S {{mirrors_num}} {{url}}
```
#### Limit download speed (bytes per second):
```shell
axel -s {{speed}} {{url}}
```
{% endraw %}