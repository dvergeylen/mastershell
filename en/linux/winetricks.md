---
layout: default
title: "winetricks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="winetricks">
  <a href="/en/linux/winetricks.html">winetricks</a> <a href="#winetricks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Wine virtual Windows environments.
> More information: <https://wiki.winehq.org/Winetricks>.

#### Start a graphical setup at the default Wine location:
```shell
winetricks
```
#### Specify a custom Wine directory to run Winetricks in:
```shell
WINEPREFIX={{path/to/wine_directory}} winetricks
```
#### Install a Windows DLL or component to the default Wine directory:
```shell
winetricks {{package}}
```
{% endraw %}