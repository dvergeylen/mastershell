---
layout: default
title: "pathchk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pathchk">
  <a href="/en/common/pathchk.html">pathchk</a> <a href="#pathchk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check the validity and portability of one or more pathnames.
> More information: <https://www.gnu.org/software/coreutils/pathchk>.

#### Check pathames for validity in the current system:
```shell
pathchk {{path1 path2 …}}
```
#### Check pathnames for validity on a wider range of POSIX compliant systems:
```shell
pathchk -p {{path1 path2 …}}
```
#### Check pathnames for validity on all POSIX compliant systems:
```shell
pathchk --portability {{path1 path2 …}}
```
#### Only check for empty pathnames or leading dashes (-):
```shell
pathchk -P {{path1 path2 …}}
```
{% endraw %}