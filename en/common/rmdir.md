---
layout: default
title: "rmdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rmdir">
  <a href="/en/common/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Removes a directory.
> More information: <https://www.gnu.org/software/coreutils/rmdir>.

#### Remove directory, provided it is empty. Use `rm -r` to remove non-empty directories:
```shell
rmdir {{path/to/directory}}
```
#### Remove the target and its parent directories (useful for nested dirs):
```shell
rmdir -p {{path/to/directory}}
```
{% endraw %}