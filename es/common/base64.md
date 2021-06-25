---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/es/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica o decodifica un archivo o la entrada estandar hacia/desde Base64, a la salida estandar.
> Más información: <https://www.gnu.org/software/coreutils/base64>.

#### Codifica un archivo:
```shell
base64 {{nombre_de_archivo}}
```
#### Decodifica un archivo:
```shell
base64 --decode {{nombre_de_archivo}}
```
#### Codifica stdin:
```shell
{{comando}} | base64
```
#### Decodifica stdin:
```shell
{{comando}} | base64 --decode
```
{% endraw %}