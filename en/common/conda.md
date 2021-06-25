---
layout: default
title: "conda"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conda">
  <a href="/en/common/conda.html">conda</a> <a href="#conda"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package, dependency and environment management for any programming language.
> More information: <https://github.com/conda/conda>.

#### Create a new environment, installing named packages into it:
```shell
conda create --name {{environment_name}} {{python=3.9 matplotlib}}
```
#### List all environments:
```shell
conda info --envs
```
#### Load an environment:
```shell
conda {{activate environment_name}}
```
#### Unload an environment:
```shell
conda {{deactivate}}
```
#### Delete an environment (remove all packages):
```shell
conda remove --name {{environment_name}} --all
```
#### Install packages into the current environment:
```shell
conda install {{python=3.4 numpy}}
```
#### List currently installed packages in current environment:
```shell
conda list
```
#### Delete unused packages and caches:
```shell
conda clean --all
```
{% endraw %}