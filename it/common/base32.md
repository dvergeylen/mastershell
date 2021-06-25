---
layout: default
title: "base32"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base32">
  <a href="/it/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica o decodifica file o standard input in Base32 su standard output.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/base32>.

#### Codifica un file:
```shell
base32 {{nome_file}}
```
#### Decodifica un file:
```shell
base32 --decode {{nome_file}}
```
#### Codifica da stdin:
```shell
{{comando}} | base32
```
#### Decodifica da stdin:
```shell
{{comando}} | base32 --decode
```
{% endraw %}