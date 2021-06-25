---
layout: default
title: "hg root"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-root">
  <a href="/en/common/hg-root.html">hg root</a> <a href="#hg-root"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the root location of a Hg repository.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#root>.

#### Display the root location of the current repository:
```shell
hg root
```
#### Display the root location of the specified repository:
```shell
hg root --cwd {{path/to/directory}}
```
{% endraw %}