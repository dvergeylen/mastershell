---
layout: default
title: "hunspell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hunspell">
  <a href="/en/common/hunspell.html">hunspell</a> <a href="#hunspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check spelling.
> More information: <https://hunspell.github.io/>.

#### Check the spelling of a file:
```shell
hunspell {{path/to/file}}
```
#### Check the spelling of a file with the en_US dictionary:
```shell
hunspell -d {{en_US}} {{path/to/file}}
```
#### List misspelled words in a file:
```shell
hunspell -l {{path/to/file}}
```
{% endraw %}