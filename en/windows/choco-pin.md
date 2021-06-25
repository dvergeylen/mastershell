---
layout: default
title: "choco pin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-pin">
  <a href="/en/windows/choco-pin.html">choco pin</a> <a href="#choco-pin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pin a package at a specific version with Chocolatey.
> Pinned packages are skipped automatically when upgrading.
> More information: <https://chocolatey.org/docs/commands-pin>.

#### Display a list of pinned packages and their versions:
```shell
choco pin list
```
#### Pin a package at its current version:
```shell
choco pin add --name {{package}}
```
#### Pin a package at a specific version:
```shell
choco pin add --name {{package}} --version {{version}}
```
#### Remove a pin for a specific package:
```shell
choco pin remove --name {{package}}
```
{% endraw %}