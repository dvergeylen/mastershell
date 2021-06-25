---
layout: default
title: "wine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wine">
  <a href="/en/linux/wine.html">wine</a> <a href="#wine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run Windows programs on Unix.
> More information: <https://wiki.winehq.org/>.

#### Run `ipconfig.exe` program:
```shell
wine {{ipconfig}} {{/all}}
```
#### Run `cmd.exe` in background:
```shell
wine start {{cmd}}
```
#### Run Windows-like Package Manager:
```shell
wine uninstaller
```
#### Install MSI packages:
```shell
wine msiexec /i {{package}}
```
{% endraw %}