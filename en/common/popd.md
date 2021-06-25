---
layout: default
title: "popd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="popd">
  <a href="/en/common/popd.html">popd</a> <a href="#popd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a directory placed on the directory stack via the pushd shell built-in.
> See also `pushd` to place a directory on the stack and `dirs` to display directory stack contents.

#### Remove the top directory from the stack and cd to it:
```shell
popd
```
#### Remove the Nth directory (starting from zero to the left from the list printed with `dirs`):
```shell
popd +N
```
#### Remove the Nth directory (starting from zero to the right from the list printed with `dirs`):
```shell
popd -N
```
{% endraw %}