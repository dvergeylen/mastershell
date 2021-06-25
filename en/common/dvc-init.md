---
layout: default
title: "dvc init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-init">
  <a href="/en/common/dvc-init.html">dvc init</a> <a href="#dvc-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Initialize a new local DVC repository.
> More information: <https://dvc.org/doc/command-reference/init>.

#### Initialize a new local repository:
```shell
dvc init
```
#### Initialize DVC without Git:
```shell
dvc init --no-scm
```
#### Initialize DVC in a subdirectory:
```shell
cd {{path/to/subdir}} && dvc init --sudir
```
{% endraw %}