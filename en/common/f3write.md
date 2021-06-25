---
layout: default
title: "f3write"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="f3write">
  <a href="/en/common/f3write.html">f3write</a> <a href="#f3write"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fill a drive out with .h2w files to test its real capacity.
> See also `f3read`, `f3probe`, `f3fix`.
> More information: <http://oss.digirati.com.br/f3/>.

#### Write test files to a given directory, filling the drive:
```shell
f3write {{path/to/mount_point}}
```
#### Limit the write speed:
```shell
f3write --max-write-rate={{kb_per_second}} {{path/to/mount_point}}
```
{% endraw %}