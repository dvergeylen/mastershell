---
layout: default
title: "poetry"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="poetry">
  <a href="/en/common/poetry.html">poetry</a> <a href="#poetry"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Python packages and dependencies.
> More information: <https://python-poetry.org/docs>.

#### Create a new Poetry project in the directory with a specific name:
```shell
poetry new {{project_name}}
```
#### Install a dependency and its subdependencies:
```shell
poetry add {{dependency}}
```
#### Interactively initialize the current directory as a new Poetry project:
```shell
poetry init
```
#### Get the latest version of all dependencies and update `poetry.lock`:
```shell
poetry update
```
#### Execute a command inside the project's virtual environment:
```shell
poetry run {{command}}
```
{% endraw %}