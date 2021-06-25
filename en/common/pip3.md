---
layout: default
title: "pip3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip3">
  <a href="/en/common/pip3.html">pip3</a> <a href="#pip3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python package manager.
> More information: <https://pip.pypa.io>.

#### Find available packages:
```shell
pip3 search {{package_name}}
```
#### Install a package:
```shell
pip3 install {{package_name}}
```
#### Install a specific version of a package:
```shell
pip3 install {{package_name}}=={{package_version}}
```
#### Upgrade a package:
```shell
pip3 install --upgrade {{package_name}}
```
#### Uninstall a package:
```shell
pip3 uninstall {{package_name}}
```
#### Save the list of installed packages to a file:
```shell
pip3 freeze > {{requirements.txt}}
```
#### Install packages from a file:
```shell
pip3 install --requirement {{requirements.txt}}
```
#### Show installed package info:
```shell
pip3 show {{package_name}}
```
{% endraw %}