---
layout: default
title: "qtchooser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qtchooser">
  <a href="/en/linux/qtchooser.html">qtchooser</a> <a href="#qtchooser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper used to select between Qt development binary versions.
> More information: <https://manned.org/qtchooser>.

#### List available Qt versions from the configuration files:
```shell
qtchooser --list-versions
```
#### Print environment information:
```shell
qtchooser --print-env
```
#### Run the specified tool using the specified Qt version:
```shell
qtchooser --run-tool={{tool}} --qt={{version_name}}
```
#### Add a Qt version entry to be able to choose from:
```shell
qtchooser --install {{version_name}} {{path/to/qmake}}
```
#### Display all available options:
```shell
qtchooser --help
```
{% endraw %}