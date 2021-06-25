---
layout: default
title: "modinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="modinfo">
  <a href="/it/linux/modinfo.html">modinfo</a> <a href="#modinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Estrae le informazioni riguardarti un modulo del kernel Linux.

#### Elenca tutti gli attributi di un modulo del kernel:
```shell
modinfo {{modulo_del_kernel}}
```
#### Elenca solamente gli attributi specificati:
```shell
modinfo -F {{author|description|license|parm|filename}} {{modulo_del_kernel}}
```
{% endraw %}