---
layout: default
title: "jupyter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jupyter">
  <a href="/en/common/jupyter.html">jupyter</a> <a href="#jupyter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web application to create and share documents that contain code, visualizations and notes.
> Primarily used for data analysis, scientific computing and machine learning.
> More information: <https://jupyter.org>.

#### Start a Jupyter notebook server in the current directory:
```shell
jupyter notebook
```
#### Open a specific Jupyter notebook:
```shell
jupyter notebook {{example.ipynb}}
```
#### Export a specific Jupyter notebook into another format:
```shell
jupyter nbconvert --to {{html|markdown|pdf|script}} {{example.ipynb}}
```
#### Start a server on a specific port:
```shell
jupyter notebook --port={{port}}
```
#### List currently running notebook servers:
```shell
jupyter notebook list
```
#### Stop the currently running server:
```shell
jupyter notebook stop
```
#### Start JupyterLab, if installed, in the current directory:
```shell
jupyter lab
```
{% endraw %}