---
layout: default
title: "flow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flow">
  <a href="/en/common/flow.html">flow</a> <a href="#flow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A static type checker for JavaScript.
> More information: <https://flow.org>.

#### Run a flow check:
```shell
flow
```
#### Check which files are being checked by flow:
```shell
flow ls
```
#### Run a type coverage check on all files in a directory:
```shell
flow batch-coverage --show-all --strip-root {{path/to/directory}}
```
#### Display line-by-line type coverage stats:
```shell
flow coverage --color {{path/to/file.jsx}}
```
{% endraw %}