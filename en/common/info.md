---
layout: default
title: "info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="info">
  <a href="/en/common/info.html">info</a> <a href="#info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reads documentation stored in the info format.
> More information: <https://en.wikipedia.org/wiki/Info_(Unix)>.

#### Start reading top-level directory menu:
```shell
info
```
#### Start reading at given menu item node from top-level directory:
```shell
info {{menu_item}}
```
#### Start reading at second menu item within first menu item manual:
```shell
info {{first_menu_item}} {{second_menu_item}}
```
{% endraw %}