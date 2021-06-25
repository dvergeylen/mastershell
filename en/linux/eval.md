---
layout: default
title: "eval"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eval">
  <a href="/en/linux/eval.html">eval</a> <a href="#eval"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute arguments as a single command in the current shell and return its result.

#### Call `echo` with the "foo" argument:
```shell
eval "{{echo foo}}"
```
#### Set a variable in the current shell:
```shell
eval "{{foo=bar}}"
```
{% endraw %}