---
layout: default
title: "rolldice"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rolldice">
  <a href="/pt_br/linux/rolldice.html">rolldice</a> <a href="#rolldice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rola dados virtuais
> Mais informações: <https://manned.org/rolldice>.

#### Rola um dado de 20 lados:
```shell
rolldice d{{20}}
```
#### Rola dois dados de seis lados e descarta o menor valor:
```shell
rolldice {{2}}d{{6}}s{{1}}
```
#### Rola dois dados de vite lados e adiciona um modificador ao resultado:
```shell
rolldice {{2}}d{{20}}{{+5}}
```
#### Rola um dado de vinte lados duas vezes:
```shell
rolldice {{2}}xd{{20}}
```
{% endraw %}