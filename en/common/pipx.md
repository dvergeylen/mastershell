---
layout: default
title: "pipx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pipx">
  <a href="/en/common/pipx.html">pipx</a> <a href="#pipx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install and run python applications in isolated environments.
> More information: <https://github.com/pipxproject/pipx>.

#### Run an app in a temporary virtual environment:
```shell
pipx run {{pycowsay}} {{moo}}
```
#### Install a package in a virtual environment and add entry points to path:
```shell
pipx install {{package}}
```
#### List installed packages:
```shell
pipx list
```
#### Run an app in a temporary virtual environment with a package name different from the executable:
```shell
pipx run --spec {{httpx-cli}} {{httpx}} {{http://www.github.com}}
```
{% endraw %}