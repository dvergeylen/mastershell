---
layout: default
title: "choco uninstall"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-uninstall">
  <a href="/en/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uninstall one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-uninstall>.

#### Uninstall one or more space-separated packages:
```shell
choco uninstall {{package(s)}}
```
#### Uninstall a specific version of a package:
```shell
choco uninstall {{package}} --version {{version}}
```
#### Confirm all prompts automatically:
```shell
choco uninstall {{package}} --yes
```
#### Remove all dependencies when uninstalling:
```shell
choco uninstall {{package}} --remove-dependencies
```
#### Uninstall all packages:
```shell
choco uninstall all
```
{% endraw %}