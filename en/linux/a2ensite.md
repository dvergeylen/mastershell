---
layout: default
title: "a2ensite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2ensite">
  <a href="/en/linux/a2ensite.html">a2ensite</a> <a href="#a2ensite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable an Apache virtual host on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2ensite.8.en.html>.

#### Enable a virtual host:
```shell
sudo a2ensite {{virtual_host}}
```
#### Don't show informative messages:
```shell
sudo a2ensite --quiet {{virtual_host}}
```
{% endraw %}