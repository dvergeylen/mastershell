---
layout: default
title: "valac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="valac">
  <a href="/en/common/valac.html">valac</a> <a href="#valac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vala code compiler.
> Tutorial: <https://wiki.gnome.org/Projects/Vala/Tutorial>.
> More information: <https://valadoc.org/>.

#### Compile a vala file, with gtk+:
```shell
valac {{path/to/file.vala}} --pkg {{gtk+-3.0}}
```
#### Display version info:
```shell
valac --version
```
#### Display helper message:
```shell
valac --help
```
{% endraw %}