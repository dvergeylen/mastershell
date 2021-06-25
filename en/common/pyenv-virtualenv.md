---
layout: default
title: "pyenv virtualenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pyenv-virtualenv">
  <a href="/en/common/pyenv-virtualenv.html">pyenv virtualenv</a> <a href="#pyenv-virtualenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create virtual environments based on one's installed Python distributions.
> More information: <https://github.com/pyenv/pyenv-virtualenv>.

#### Create a new Python 3.6.6 virtual environment:
```shell
pyenv virtualenv {{3.6.6}} {{virtualenv_name}}
```
#### List all existing virtual environments:
```shell
pyenv virtualenvs
```
#### Activate a virtual environment:
```shell
pyenv activate {{virtualenv_name}}
```
#### Deactivate the virtual environment:
```shell
pyenv deactivate
```
{% endraw %}