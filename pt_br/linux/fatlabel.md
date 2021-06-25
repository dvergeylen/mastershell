---
layout: default
title: "fatlabel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fatlabel">
  <a href="/pt_br/linux/fatlabel.html">fatlabel</a> <a href="#fatlabel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Define ou exibe o rótulo de uma partição FAT32.

#### Exibir o rótulo de uma partição FAT32:
```shell
fatlabel {{/dev/sda1}}
```
#### Definir o rótulo de uma partição FAT32:
```shell
fatlabel {{/dev/sdc3}} "{{rotulo}}"
```
{% endraw %}