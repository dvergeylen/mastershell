---
layout: default
title: "jupytext"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jupytext">
  <a href="/en/common/jupytext.html">jupytext</a> <a href="#jupytext"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to convert Jupyter notebooks to plain text documents, and back again.
> More information: <https://jupytext.readthedocs.io/en/latest/>.

#### Turn a notebook into a paired `.ipynb`/`.py` notebook:
```shell
jupytext --set-formats ipynb,py {{notebook.ipynb}}
```
#### Convert a notebook to a `.py` file:
```shell
jupytext --to py {{notebook.ipynb}}
```
#### Convert a `.py` file to a notebook with no outputs:
```shell
jupytext --to notebook {{notebook.py}}
```
#### Convert a `.md` file to a notebook and run it:
```shell
jupytext --to notebook --execute {{notebook.md}}
```
#### Update the input cells in a notebook and preserve outputs and metadata:
```shell
jupytext --update --to notebook {{notebook.py}}
```
#### Update all paired representations of a notebook:
```shell
jupytext --sync {{notebook.ipynb}}
```
{% endraw %}