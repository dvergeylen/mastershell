---
layout: default
title: "doxygen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doxygen">
  <a href="/en/common/doxygen.html">doxygen</a> <a href="#doxygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A documentation system for various programming languages.
> More information: <http://www.doxygen.nl>.

#### Generate a default template configuration file `Doxyfile`:
```shell
doxygen -g
```
#### Generate a template configuration file:
```shell
doxygen -g {{path/to/config_file}}
```
#### Generate documentation using an existing configuration file:
```shell
doxygen {{path/to/config_file}}
```
{% endraw %}