---
layout: default
title: "gops"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gops">
  <a href="/en/common/gops.html">gops</a> <a href="#gops"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI tool which lists and diagnoses Go processes currently running on your system.
> More information: <https://github.com/google/gops>.

#### Print all go processes running locally:
```shell
gops
```
#### Print more information about a process:
```shell
gops {{pid}}
```
#### Display a process tree:
```shell
gops tree
```
#### Print the current stack trace from a target program:
```shell
gops stack {{pid|addr}}
```
#### Print the current runtime memory statistics:
```shell
gops memstats {{pid|addr}}
```
{% endraw %}