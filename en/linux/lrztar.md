---
layout: default
title: "lrztar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lrztar">
  <a href="/en/linux/lrztar.html">lrztar</a> <a href="#lrztar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper for `lrzip` to simplify compression of directories.
> See also: `tar`, `lrzuntar`, `lrunzip`.

#### Archive a directory with `tar`, then compress:
```shell
lrztar {{path/to/directory}}
```
#### Same as above, with ZPAQ - extreme compression, but very slow:
```shell
lrztar -z {{path/to/directory}}
```
#### Specify the output file:
```shell
lrztar -o {{path/to/file}} {{path/to/directory}}
```
#### Override the number of processor threads to use:
```shell
lrztar -p {{8}} {{path/to/directory}}
```
#### Force overwriting of existing files:
```shell
lrztar -f {{path/to/directory}}
```
{% endraw %}