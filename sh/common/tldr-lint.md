---
layout: default
title: "tldr-lint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr-lint">
  <a href="/sh/common/tldr-lint.html">tldr-lint</a> <a href="#tldr-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lintuje i formatira tldr stranice.
> Više informacija: <https://github.com/tldr-pages/tldr-lint>.

#### Lintuj sve stranice:
```shell
tldr-lint {{direktorijum_stranica}}
```
#### Formatiraj određenu stranicu u stdout:
```shell
tldr-lint --format {{stranica.md}}
```
#### Formatiraj sve stranice na njihovom mestu:
```shell
tldr-lint --format --in-place {{direktorijum_stranica}}
```
{% endraw %}