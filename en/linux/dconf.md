---
layout: default
title: "dconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dconf">
  <a href="/en/linux/dconf.html">dconf</a> <a href="#dconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple tool for manipulating dconf databases.
> See also `dconf write`.
> More information: <https://developer.gnome.org/dconf>.

#### Print the value of a dconf path:
```shell
dconf read {{/example/dconf/path}}
```
#### List contents of a dconf path:
```shell
dconf list {{/example/dconf/path}}
```
#### Watch for dconf database changes in a path and subpaths:
```shell
dconf watch {{/example/dconf/path}}
```
{% endraw %}