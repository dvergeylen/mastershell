---
layout: default
title: "pipenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pipenv">
  <a href="/en/common/pipenv.html">pipenv</a> <a href="#pipenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple and unified Python development workflow.
> Manages packages and the virtual environment for a project.
> More information: <https://pypi.org/project/pipenv>.

#### Create a new project:
```shell
pipenv
```
#### Create a new project using Python 3:
```shell
pipenv --three
```
#### Install a package:
```shell
pipenv install {{package_name}}
```
#### Install all the dependencies for a project:
```shell
pipenv install
```
#### Install all the dependencies for a project (including dev packages):
```shell
pipenv install --dev
```
#### Uninstall a package:
```shell
pipenv uninstall {{package_name}}
```
#### Start a shell within the created virtual environment:
```shell
pipenv shell
```
#### Generate a `requirements.txt` (list of dependencies) for a project:
```shell
pipenv lock --requirements
```
{% endraw %}