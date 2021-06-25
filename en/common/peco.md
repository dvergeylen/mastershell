---
layout: default
title: "peco"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="peco">
  <a href="/en/common/peco.html">peco</a> <a href="#peco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactive filtering tool.
> More information: <https://github.com/peco/peco>.

#### Start peco on all files in the specified directory:
```shell
find {{path/to/directory}} -type f | peco
```
#### Start peco for running processes:
```shell
ps aux | peco
```
#### Start peco with a specified query:
```shell
peco --query "{{query}}"
```
{% endraw %}