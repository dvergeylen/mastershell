---
layout: default
title: "debman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debman">
  <a href="/en/linux/debman.html">debman</a> <a href="#debman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read man pages from uninstalled packages.

#### Read a man page for a command that is provided by a specified package name:
```shell
debman -p {{package_name}} {{command_name}}
```
#### Specify a package version to download:
```shell
debman -p {{package_name}}={{version}} {{command_name}}
```
#### Read a man page in a `.deb` file:
```shell
debman -f {{path/to/filename.deb}} {{command_name}}
```
{% endraw %}