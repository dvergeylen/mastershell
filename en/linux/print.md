---
layout: default
title: "print"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="print">
  <a href="/en/linux/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alias to a `run-mailcap`'s action print.
> Originally `run-mailcap` is used to process mime-type/file.

#### Print action can be used to print any file on default run-mailcap tool:
```shell
print {{filename}}
```
#### With `run-mailcap`:
```shell
run-mailcap --action=print {{filename}}
```
{% endraw %}