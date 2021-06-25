---
layout: default
title: "fnm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fnm">
  <a href="/en/common/fnm.html">fnm</a> <a href="#fnm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fast Node.js version manager.
> Install, uninstall or switch between Node.js versions.
> More information: <https://github.com/Schniz/fnm>.

#### Install a specific version of Node.js:
```shell
fnm install {{node_version}}
```
#### List all available Node.js versions and highlight the default one:
```shell
fnm ls
```
#### Use a specific version of Node.js in the current shell:
```shell
fnm use {{node_version}}
```
#### Set the default Node.js version:
```shell
fnm default {{node_version}}
```
#### Uninstall a given Node.js version:
```shell
fnm uninstall {{node_version}}
```
{% endraw %}