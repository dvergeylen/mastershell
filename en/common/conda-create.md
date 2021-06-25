---
layout: default
title: "conda create"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conda-create">
  <a href="/en/common/conda-create.html">conda create</a> <a href="#conda-create"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create new conda environments.
> More information: <https://docs.conda.io/projects/conda/en/latest/commands/create.html>.

#### Create a new environment named `py39`, and install Python 3.9 and numpy v1.11 or above in it:
```shell
conda create --yes --name {{py39}} python={{3.9}} "{{numpy>=1.11}}"
```
#### Make exact copy of an environment:
```shell
conda create --clone {{py39}} --name {{py39-copy}}
```
#### Create a new environment with a specified name and install a given package:
```shell
conda create --name {{env_name}} {{package_name}}
```
{% endraw %}