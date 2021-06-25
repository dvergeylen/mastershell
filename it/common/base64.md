---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/it/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica o decodifica file o standard input in Base64 su standard output.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/base64>.

#### Codifica un file:
```shell
base64 {{nome_file}}
```
#### Decodifica un file:
```shell
base64 --decode {{nome_file}}
```
#### Codifica da stdin:
```shell
{{comando}} | base64
```
#### Decodifica da stdin:
```shell
{{comando}} | base64 --decode
```
{% endraw %}