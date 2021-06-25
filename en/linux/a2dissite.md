---
layout: default
title: "a2dissite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dissite">
  <a href="/en/linux/a2dissite.html">a2dissite</a> <a href="#a2dissite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable an Apache virtual host on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2dissite.8.en.html>.

#### Disable a virtual host:
```shell
sudo a2dissite {{virtual_host}}
```
#### Don't show informative messages:
```shell
sudo a2dissite --quiet {{virtual_host}}
```
{% endraw %}