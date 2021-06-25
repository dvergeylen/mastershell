---
layout: default
title: "phpenmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpenmod">
  <a href="/en/linux/phpenmod.html">phpenmod</a> <a href="#phpenmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable PHP extensions on Debian-based OSes.

#### Enable the json extension for every SAPI of every PHP version:
```shell
sudo phpenmod {{json}}
```
#### Enable the json extension for PHP 7.3 with the cli SAPI:
```shell
sudo phpenmod -v {{7.3}} -s {{cli}} {{json}}
```
{% endraw %}