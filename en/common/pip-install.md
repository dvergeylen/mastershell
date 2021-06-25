---
layout: default
title: "pip install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pip-install">
  <a href="/en/common/pip-install.html">pip install</a> <a href="#pip-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install Python packages.
> More information: <https://pip.pypa.io>.

#### Install a package:
```shell
pip install {{package_name}}
```
#### Install a specific version of a package:
```shell
pip install {{package_name}}=={{package_version}}
```
#### Install packages listed in a file:
```shell
pip install -r {{requirements.txt}}
```
#### Install the local package in the current directory in develop (editable) mode:
```shell
pip install -e .
```
{% endraw %}