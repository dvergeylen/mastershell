---
layout: default
title: "pip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip">
  <a href="/en/common/pip.html">pip</a> <a href="#pip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python package manager.
> More information: <https://pip.pypa.io>.

#### Install a package (see `pip install` for more install examples):
```shell
pip install {{package_name}}
```
#### Upgrade a package:
```shell
pip install -U {{package_name}}
```
#### Uninstall a package:
```shell
pip uninstall {{package_name}}
```
#### Save installed packages to file:
```shell
pip freeze > {{requirements.txt}}
```
#### Show installed package info:
```shell
pip show {{package_name}}
```
{% endraw %}