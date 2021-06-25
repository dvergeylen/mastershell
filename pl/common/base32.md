---
layout: default
title: "base32"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base32">
  <a href="/pl/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enkoduj lub dekoduj plik lub standardowe wejście do/z Base32, na standardowe wyjście.
> Więcej informacji: <https://www.gnu.org/software/coreutils/base32>.

#### Enkoduj plik:
```shell
base32 {{nazwapliku}}
```
#### Dekoduj plik:
```shell
base32 --decode {{nazwapliku}}
```
#### Enkoduj z stdin:
```shell
{{jakiespolecenie}} | base32
```
#### Dekoduj z stdin:
```shell
{{jakiespolecenie}} | base32 --decode
```
{% endraw %}