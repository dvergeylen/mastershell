---
layout: default
title: "cmp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmp">
  <a href="/en/common/cmp.html">cmp</a> <a href="#cmp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare two files byte by byte.
> More information: <https://www.gnu.org/software/diffutils/manual/html_node/Invoking-cmp.html>.

#### Find the byte and line number of the first difference between two files:
```shell
cmp {{path/to/file1}} {{path/to/file2}}
```
#### Find the byte number and differing bytes of every difference:
```shell
cmp -l {{path/to/file1}} {{path/to/file2}}
```
{% endraw %}