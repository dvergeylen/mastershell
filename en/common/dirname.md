---
layout: default
title: "dirname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirname">
  <a href="/en/common/dirname.html">dirname</a> <a href="#dirname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculates the parent directory of a given file or directory path.
> More information: <https://www.gnu.org/software/coreutils/dirname>.

#### Calculate the parent directory of a given path:
```shell
dirname {{path/to/file_or_directory}}
```
#### Calculate the parent directory of multiple paths:
```shell
dirname {{path/to/file_a}} {{path/to/directory_b}}
```
#### Delimit output with a NUL character instead of a newline (useful when combining with `xargs`):
```shell
dirname --zero {{path/to/directory_a}} {{path/to/file_b}}
```
{% endraw %}