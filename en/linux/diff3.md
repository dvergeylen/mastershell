---
layout: default
title: "diff3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diff3">
  <a href="/en/linux/diff3.html">diff3</a> <a href="#diff3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare three files line by line.

#### Compare files:
```shell
diff3 {{file1}} {{file2}} {{file3}}
```
#### Show all changes, outlining conflicts:
```shell
diff3 --show-all {{file1}} {{file2}} {{file3}}
```
{% endraw %}