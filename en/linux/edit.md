---
layout: default
title: "edit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="edit">
  <a href="/en/linux/edit.html">edit</a> <a href="#edit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alias to a `run-mailcap`'s action edit.
> Originally `run-mailcap` is used to process/edit mime-type/file.

#### Edit action can be used to view any file on default mailcap explorer:
```shell
edit {{filename}}
```
#### With `run-mailcap`:
```shell
run-mailcap --action=edit {{filename}}
```
{% endraw %}