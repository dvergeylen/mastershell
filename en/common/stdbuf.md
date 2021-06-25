---
layout: default
title: "stdbuf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stdbuf">
  <a href="/en/common/stdbuf.html">stdbuf</a> <a href="#stdbuf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command with modified buffering operations for its standard streams.
> More information: <https://www.gnu.org/software/coreutils/stdbuf>.

#### Change the standard input buffer size to 512 KiB:
```shell
stdbuf --input={{512K}} {{command}}
```
#### Change the standard output buffer to line-buffered:
```shell
stdbuf --output={{L}} {{command}}
```
#### Change the standard error buffer to unbuffered:
```shell
stdbuf --error={{0}} {{command}}
```
{% endraw %}