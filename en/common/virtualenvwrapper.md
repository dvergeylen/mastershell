---
layout: default
title: "virtualenvwrapper"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virtualenvwrapper">
  <a href="/en/common/virtualenvwrapper.html">virtualenvwrapper</a> <a href="#virtualenvwrapper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Group of simple wrapper commands for Python's `virtualenv` tool.
> More information: <http://virtualenvwrapper.readthedocs.org>.

#### Create a new Python `virtualenv` in `$WORKON_HOME`:
```shell
mkvirtualenv {{virtualenv_name}}
```
#### Create a `virtualenv` for a specific Python version:
```shell
mkvirtualenv --python {{/usr/local/bin/python3.8}} {{virtualenv_name}}
```
#### Activate or use a different `virtualenv`:
```shell
workon {{virtualenv_name}}
```
#### Stop the `virtualenv`:
```shell
deactivate
```
#### List all virtual environments:
```shell
lsvirtualenv
```
#### Remove a `virtualenv`:
```shell
rmvirtualenv {{virtualenv_name}}
```
#### Get summary of all virtualenvwrapper commands:
```shell
virtualenvwrapper
```
{% endraw %}