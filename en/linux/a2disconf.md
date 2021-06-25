---
layout: default
title: "a2disconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2disconf">
  <a href="/en/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable an Apache configuration file on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2disconf.8.en.html>.

#### Disable a configuration file:
```shell
sudo a2disconf {{configuration_file}}
```
#### Don't show informative messages:
```shell
sudo a2disconf --quiet {{configuration_file}}
```
{% endraw %}