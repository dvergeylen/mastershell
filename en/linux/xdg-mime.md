---
layout: default
title: "xdg-mime"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xdg-mime">
  <a href="/en/linux/xdg-mime.html">xdg-mime</a> <a href="#xdg-mime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query and manage MIME types according to the XDG standard.
> More information: <https://portland.freedesktop.org/doc/xdg-mime.html>.

#### Display the MIME type of a file:
```shell
xdg-mime query filetype {{path/to/file}}
```
#### Display the default application for opening PNG images:
```shell
xdg-mime query default {{image/png}}
```
#### Display the default application for opening a specific file:
```shell
xdg-mime query default $(xdg-mime query filetype {{path/to/file}})
```
#### Set imv as the default application for opening PNG and JPEG images:
```shell
xdg-mime default {{imv.desktop}} {{image/png}} {{image/jpeg}}
```
{% endraw %}