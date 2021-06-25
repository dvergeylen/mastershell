---
layout: default
title: "pyenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pyenv">
  <a href="/en/common/pyenv.html">pyenv</a> <a href="#pyenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch between multiple versions of Python easily.
> More information: <https://github.com/pyenv/pyenv>.

#### List all available commands:
```shell
pyenv commands
```
#### List all Python versions under the `${PYENV_ROOT}/versions` directory:
```shell
pyenv versions
```
#### Install a Python version under the `${PYENV_ROOT}/versions` directory:
```shell
pyenv install {{2.7.10}}
```
#### Uninstall a Python version under the `${PYENV_ROOT}/versions` directory:
```shell
pyenv uninstall {{2.7.10}}
```
#### Set Python version to be used globally in the current machine:
```shell
pyenv global {{2.7.10}}
```
#### Set Python version to be used in the current directory and all directories below it:
```shell
pyenv local {{2.7.10}}
```
{% endraw %}