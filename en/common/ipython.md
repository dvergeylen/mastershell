---
layout: default
title: "IPython"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipython">
  <a href="/en/common/ipython.html">IPython</a> <a href="#ipython"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Python shell with automatic history, dynamic object introspection, easier configuration, command completion, access to the system shell and more.
> More information: <https://ipython.org/documentation.html>.

#### Start an interactive IPython session:
```shell
ipython
```
#### Enter an interactive IPython session after running a Python script:
```shell
ipython -i {{script.py}}
```
#### Create default IPython profile:
```shell
ipython profile create
```
#### Print the path to the directory for the default IPython profile:
```shell
ipython locate profile
```
#### Clear the IPython history database, deleting all entries:
```shell
ipython history clear
```
{% endraw %}