---
layout: default
title: "glib-compile-resources"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="glib-compile-resources">
  <a href="/en/common/glib-compile-resources.html">glib-compile-resources</a> <a href="#glib-compile-resources"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compiles resource files (e.g. images) into a binary resource bundle.
> These may be linked into GTK applications using the GResource API.
> More information: <https://manned.org/glib-compile-resources>.

#### Compile resources referenced in `file.gresource.xml` to a .gresource binary:
```shell
glib-compile-resources {{file.gresource.xml}}
```
#### Compile resources referenced in `file.gresource.xml` to a C source file:
```shell
glib-compile-resources --generate-source {{file.gresource.xml}}
```
#### Compile resources in `file.gresource.xml` to a chosen target file, with `.c`, `.h` or `.gresource` extension:
```shell
glib-compile-resources --generate --target={{file.ext}} {{file.gresource.xml}}
```
#### Print a list of resource files referenced in `file.gresource.xml`:
```shell
glib-compile-resources --generate-dependencies {{file.gresource.xml}}
```
{% endraw %}