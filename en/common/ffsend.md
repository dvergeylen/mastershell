---
layout: default
title: "ffsend"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ffsend">
  <a href="/en/common/ffsend.html">ffsend</a> <a href="#ffsend"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Easily and securely share files from command-line.
> More information: <https://gitlab.com/timvisee/ffsend>.

#### Upload a file:
```shell
ffsend upload {{file}}
```
#### Download a file:
```shell
ffsend download {{url}}
```
#### Upload a file with password:
```shell
ffsend upload {{file}} -p {{password}}
```
#### Download a file protected by password:
```shell
ffsend download {{file}} -p {{password}}
```
#### Upload a file and allow 4 downloads:
```shell
ffsend upload {{file}} -d {{4}}
```
{% endraw %}