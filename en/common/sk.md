---
layout: default
title: "sk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sk">
  <a href="/en/common/sk.html">sk</a> <a href="#sk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fuzzy finder written in Rust.
> Similar to `fzf`.
> More information: <https://github.com/lotabout/skim>.

#### Start skim on all files in the specified directory:
```shell
find {{path/to/directory}} -type f | sk
```
#### Start skim for running processes:
```shell
ps aux | sk
```
#### Start skim with a specified query:
```shell
sk --query "{{query}}"
```
#### Select multiple files with `Shift + Tab` and write to a file:
```shell
find {{path/to/directory}} -type f | sk --multi > {{filename}}
```
{% endraw %}