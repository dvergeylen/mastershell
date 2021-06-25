---
layout: default
title: "xdg-open"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xdg-open">
  <a href="/en/linux/xdg-open.html">xdg-open</a> <a href="#xdg-open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens a file or URL in the user's preferred application.
> More information: <https://man.archlinux.org/man/xdg-open.1>.

#### Open the current directory in the default file explorer:
```shell
xdg-open .
```
#### Open an URL in the default browser:
```shell
xdg-open {{https://example.com}}
```
#### Open an image in the default image viewer:
```shell
xdg-open {{path/to/image}}
```
#### Open a PDF in the default PDF viewer:
```shell
xdg-open {{path/to/pdf}}
```
#### Display help:
```shell
xdg-open --help
```
{% endraw %}