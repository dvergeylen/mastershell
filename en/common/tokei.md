---
layout: default
title: "tokei"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tokei">
  <a href="/en/common/tokei.html">tokei</a> <a href="#tokei"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A program that prints out statistics about code.
> More information: <https://github.com/XAMPPRocky/tokei>.

#### Get a report on the code in a directory and all subdirectories:
```shell
tokei {{path/to/directory}}
```
#### Get a report for a directory excluding `.min.js` files:
```shell
tokei {{path/to/directory}} -e {{*.min.js}}
```
#### Print out statistics for individual files in a directory:
```shell
tokei {{path/to/directory}} --files
```
#### Get a report for all files of type Rust and Markdown:
```shell
tokei {{path/to/directory}} -t={{Rust}},{{Markdown}}
```
{% endraw %}