---
layout: default
title: "fisher"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fisher">
  <a href="/en/common/fisher.html">fisher</a> <a href="#fisher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fisher, a fish-shell plugin manager.
> Install plugins by name or from a managed 'fishfile' for bundled installs.
> More information: <https://github.com/jorgebucaran/fisher>.

#### Install one or more plugins:
```shell
fisher {{plugin1}} {{plugin2}}
```
#### Install a plugin from a GitHub gist:
```shell
fisher {{gist_url}}
```
#### Edit 'fishfile' by hand with your favorite editor and install multiple plugins:
```shell
{{editor}} ~/.config/fish/fishfile; fisher
```
#### List installed plugins:
```shell
fisher ls
```
#### Update plugins:
```shell
fisher update
```
#### Remove one or more plugins:
```shell
fisher remove {{plugin1}} {{plugin2}}
```
{% endraw %}