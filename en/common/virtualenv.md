---
layout: default
title: "virtualenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virtualenv">
  <a href="/en/common/virtualenv.html">virtualenv</a> <a href="#virtualenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create virtual isolated Python environments.
> More information: <https://virtualenv.pypa.io/>.

#### Create a new environment:
```shell
virtualenv {{path/to/venv}}
```
#### Customize the prompt prefix:
```shell
virtualenv --prompt={{prompt_prefix}} {{path/to/venv}}
```
#### Use a different version of Python with virtualenv:
```shell
virtualenv --python={{path/to/pythonbin}} {{path/to/venv}}
```
#### Start (select) the environment:
```shell
source {{path/to/venv}}/bin/activate
```
#### Stop the environment:
```shell
deactivate
```
{% endraw %}