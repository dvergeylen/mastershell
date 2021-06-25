---
layout: default
title: "pushd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pushd">
  <a href="/en/common/pushd.html">pushd</a> <a href="#pushd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Place a directory on a stack so it can be accessed later.
> See also `popd` to switch back to original directory and `dirs` to display directory stack contents.

#### Switch to directory and push it on the stack:
```shell
pushd {{directory}}
```
#### Switch first and second directories on the stack:
```shell
pushd
```
#### Rotate stack by making the 5th element the top of the stack:
```shell
pushd +4
```
{% endraw %}