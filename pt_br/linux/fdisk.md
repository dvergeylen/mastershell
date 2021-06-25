---
layout: default
title: "fdisk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdisk">
  <a href="/pt_br/linux/fdisk.html">fdisk</a> <a href="#fdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de tabelas de partições e partições no disco rígido.

#### Exibir as partições:
```shell
fdisk -l
```
#### Iniciar o manipulador de partições:
```shell
fdisk {{/dev/sda}}
```
{% endraw %}