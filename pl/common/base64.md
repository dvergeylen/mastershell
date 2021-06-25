---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/pl/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enkoduj lub dekoduj plik lub standardowe wejście do/z Base64, na standardowe wyjście.
> Więcej informacji: <https://www.gnu.org/software/coreutils/base64>.

#### Enkoduj plik:
```shell
base64 {{nazwapliku}}
```
#### Dekoduj plik:
```shell
base64 --decode {{nazwapliku}}
```
#### Enkoduj z stdin:
```shell
{{jakiespolecenie}} | base64
```
#### Dekoduj z stdin:
```shell
{{jakiespolecenie}} | base64 --decode
```
{% endraw %}