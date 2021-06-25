---
layout: default
title: "astronomer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="astronomer">
  <a href="/pl/common/astronomer.html">astronomer</a> <a href="#astronomer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie wykrywające nielegalne gwiazdki z kont botów w projektach GithHub.
> Więcej informacji: <https://github.com/Ullaakut/astronomer>.

#### Skanuj repozytorium:
```shell
astronomer {{tldr-pages/tldr-node-client}}
```
#### Zeskanuj maksymalną liczbę gwiazdek w repozytorium:
```shell
astronomer {{tldr-pages/tldr-node-client}} --stars {{50}}
```
#### Przeskanuj repozytorium, w tym raporty porównawcze:
```shell
astronomer {{tldr-pages/tldr-node-client}} --verbose
```
{% endraw %}