---
layout: default
title: "pre-commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pre-commit">
  <a href="/en/common/pre-commit.html">pre-commit</a> <a href="#pre-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create Git hooks that get run before a commit.
> More information: <https://pre-commit.com>.

#### Install pre-commit into your Git hooks:
```shell
pre-commit install
```
#### Run pre-commit hooks on all staged files:
```shell
pre-commit run
```
#### Run pre-commit hooks on all files, staged or unstaged:
```shell
pre-commit run --all-files
```
#### Clean pre-commit cache:
```shell
pre-commit clean
```
{% endraw %}