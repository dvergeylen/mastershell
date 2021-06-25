---
layout: default
title: "pkg-config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkg-config">
  <a href="/en/linux/pkg-config.html">pkg-config</a> <a href="#pkg-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provide the details of installed libraries for compiling applications.
> More information: <https://www.freedesktop.org/wiki/Software/pkg-config/>.

#### Get the list of libraries and their dependencies:
```shell
pkg-config --libs {{library1 library2 ...}}
```
#### Get the list of libraries, their dependencies, and proper cflags for gcc:
```shell
pkg-config --cflags --libs {{library1 library2 ...}}
```
#### Compile your code with libgtk-3, libwebkit2gtk-4.0 and all their dependencies:
```shell
c++ example.cpp $(pkg-config --cflags --libs gtk+-3.0 webkit2gtk-4.0) -o example
```
{% endraw %}