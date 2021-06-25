---
layout: default
title: "phpdismod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpdismod">
  <a href="/en/linux/phpdismod.html">phpdismod</a> <a href="#phpdismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable PHP extensions on Debian-based OSes.

#### Disable the json extension for every SAPI of every PHP version:
```shell
sudo phpdismod {{json}}
```
#### Disable the json extension for PHP 7.3 with the cli SAPI:
```shell
sudo phpdismod -v {{7.3}} -s {{cli}} {{json}}
```
{% endraw %}