---
layout: default
title: "astronomer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="astronomer">
  <a href="/it/common/astronomer.html">astronomer</a> <a href="#astronomer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per individuare star illegittime da account bot su progetti GitHub.
> Maggiori informazioni: <https://github.com/Ullaakut/astronomer>.

#### Scannerizza una repository:
```shell
astronomer {{tldr-pages/tldr-node-client}}
```
#### Scannerizza le star di una repository fino ad un massimo di 50:
```shell
astronomer {{tldr-pages/tldr-node-client}} --stars {{50}}
```
#### Scannerizza una repository includendo report comparativi:
```shell
astronomer {{tldr-pages/tldr-node-client}} --verbose
```
{% endraw %}