---
layout: default
title: "astronomer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="astronomer">
  <a href="/en/common/astronomer.html">astronomer</a> <a href="#astronomer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool that detects illegitimate stars from bot accounts on GitHub projects.
> More information: <https://github.com/Ullaakut/astronomer>.

#### Scan a repository:
```shell
astronomer {{tldr-pages/tldr-node-client}}
```
#### Scan the maximum amount of stars in the repository:
```shell
astronomer {{tldr-pages/tldr-node-client}} --stars {{50}}
```
#### Scan a repository including comparative reports:
```shell
astronomer {{tldr-pages/tldr-node-client}} --verbose
```
{% endraw %}