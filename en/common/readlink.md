---
layout: default
title: "readlink"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="readlink">
  <a href="/en/common/readlink.html">readlink</a> <a href="#readlink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Follow symlinks and get symlink information.
> More information: <https://www.gnu.org/software/coreutils/readlink>.

#### Get the actual file to which the symlink points:
```shell
readlink {{filename}}
```
#### Get the absolute path to a file:
```shell
readlink -f {{filename}}
```
{% endraw %}