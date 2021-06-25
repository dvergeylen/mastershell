---
layout: default
title: "mkdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkdir">
  <a href="/en/common/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a directory.
> More information: <https://www.gnu.org/software/coreutils/mkdir>.

#### Create a directory in current directory or given path:
```shell
mkdir {{directory}}
```
#### Create directories recursively (useful for creating nested dirs):
```shell
mkdir -p {{path/to/directory}}
```
{% endraw %}