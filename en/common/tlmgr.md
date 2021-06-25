---
layout: default
title: "tlmgr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tlmgr">
  <a href="/en/common/tlmgr.html">tlmgr</a> <a href="#tlmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manages packages and configuration options of an existing TeX Live installation.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

#### Install a package and its dependencies:
```shell
tlmgr install {{package}}
```
#### Remove a package and its dependencies:
```shell
tlmgr remove {{package}}
```
#### Display information about a package:
```shell
tlmgr info {{package}}
```
#### Update all packages:
```shell
tlmgr update --all
```
#### Show possible updates without updating anything:
```shell
tlmgr update --list
```
#### Start a GUI version of tlmgr:
```shell
tlmgr gui
```
#### List all TeX Live configurations:
```shell
tlmgr conf
```
{% endraw %}