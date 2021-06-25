---
layout: default
title: "python"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="python">
  <a href="/en/common/python.html">python</a> <a href="#python"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python language interpreter.
> More information: <https://www.python.org>.

#### Call a Python interactive shell (REPL):
```shell
python
```
#### Execute script in a given Python file:
```shell
python {{script.py}}
```
#### Execute script as part of an interactive shell:
```shell
python -i {{script.py}}
```
#### Execute a Python expression:
```shell
python -c "{{expression}}"
```
#### Run library module as a script (terminates option list):
```shell
python -m {{module}} {{arguments}}
```
#### Install a package using pip:
```shell
python -m pip install {{package_name}}
```
#### Interactively debug a Python script:
```shell
python -m pdb {{script.py}}
```
{% endraw %}