---
layout: default
title: "kreadconfig5"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kreadconfig5">
  <a href="/en/linux/kreadconfig5.html">kreadconfig5</a> <a href="#kreadconfig5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read KConfig entries for KDE Plasma.
> More information: <https://userbase.kde.org/KDE_System_Administration/Configuration_Files>.

#### Read a key from the global configuration:
```shell
kreadconfig5 --group {{group_name}} --key {{key_name}}
```
#### Read a key from a specific configuration file:
```shell
kwriteconfig5 --file {{path/to/file}} --group {{group_name}} --key {{key_name}}
```
#### Check if systemd is used to start the Plasma session:
```shell
kreadconfig5 --file {{startkderc}} --group {{General}} --key {{systemdBoot}}
```
{% endraw %}