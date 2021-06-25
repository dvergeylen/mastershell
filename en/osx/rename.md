---
layout: default
title: "rename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rename">
  <a href="/en/osx/rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename a file or group of files with a regular expression.

#### Replace `from` with `to` in the filenames of the specified files:
```shell
rename 's/{{from}}/{{to}}/' {{*.txt}}
```
{% endraw %}