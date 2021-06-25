---
layout: default
title: "chflags"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chflags">
  <a href="/en/osx/chflags.html">chflags</a> <a href="#chflags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change file or directory flags.

#### Set the `hidden` flag for a file:
```shell
chflags {{hidden}} {{path/to/file}}
```
#### Unset the `hidden` flag for a file:
```shell
chflags {{nohidden}} {{path/to/file}}
```
#### Recursively set the `uchg` flag for a directory:
```shell
chflags -R {{uchg}} {{path/to/directory}}
```
#### Recursively unset the `uchg` flag for a directory:
```shell
chflags -R {{nouchg}} {{path/to/directory}}
```
{% endraw %}