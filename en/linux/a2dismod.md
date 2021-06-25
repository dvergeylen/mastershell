---
layout: default
title: "a2dismod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dismod">
  <a href="/en/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable an Apache module on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2dismod.8.en.html>.

#### Disable a module:
```shell
sudo a2dismod {{module}}
```
#### Don't show informative messages:
```shell
sudo a2dismod --quiet {{module}}
```
{% endraw %}