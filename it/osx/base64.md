---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/it/osx/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica e decodifica utilizzando la rappresentazione in base64.

#### Codifica un file:
```shell
base64 -i {{file_da_codificare}}
```
#### Decodifica un file:
```shell
base64 --decode -i {{file_da_decodificare}}
```
#### Codifica da stdin:
```shell
echo -n {{testo_da_codificare}} | base64
```
#### Decodifica da stdin:
```shell
echo -n {{testo_da_decodificare}} | base64 --decode
```
{% endraw %}