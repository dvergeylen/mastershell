---
layout: default
title: "a2enconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2enconf">
  <a href="/en/linux/a2enconf.html">a2enconf</a> <a href="#a2enconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable an Apache configuration file on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2enconf.8.en.html>.

#### Enable a configuration file:
```shell
sudo a2enconf {{configuration_file}}
```
#### Don't show informative messages:
```shell
sudo a2enconf --quiet {{configuration_file}}
```
{% endraw %}