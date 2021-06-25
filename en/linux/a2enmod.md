---
layout: default
title: "a2enmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2enmod">
  <a href="/en/linux/a2enmod.html">a2enmod</a> <a href="#a2enmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable an Apache module on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2enmod.8.en.html>.

#### Enable a module:
```shell
sudo a2enmod {{module}}
```
#### Don't show informative messages:
```shell
sudo a2enmod --quiet {{module}}
```
{% endraw %}