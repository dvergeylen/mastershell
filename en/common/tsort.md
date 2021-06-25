---
layout: default
title: "tsort"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tsort">
  <a href="/en/common/tsort.html">tsort</a> <a href="#tsort"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform a topological sort.
> A common use is to show the dependency order of nodes in a directed acyclic graph.
> More information: <https://www.gnu.org/software/coreutils/tsort>.

#### Perform a topological sort consistent with a partial sort per line of input separated by blanks:
```shell
tsort {{file}}
```
{% endraw %}