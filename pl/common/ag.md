---
layout: default
title: "ag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ag">
  <a href="/pl/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. Podobny do ack, ale ma być szybszy.
> Więcej informacji: <https://github.com/ggreer/the_silver_searcher>.

#### Znajdź pliki zawierające „foo” i wypisz dopasowane linie:
```shell
ag {{foo}}
```
#### Znajdź pliki zawierające „foo” w określonym katalogu:
```shell
ag {{foo}} {{scieżka/do/katalogu}}
```
#### Znajdź pliki zawierające „foo”, ale podaj tylko nazwy plików:
```shell
ag -l {{foo}}
```
#### Znajdź pliki zawierające „FOO” bez rozróżniania wielkości liter i wypisz tylko dopasowanie, a nie całą linię:
```shell
ag -i -o {{FOO}}
```
#### Znajdź „foo” w plikach o nazwie pasującej do „bar”:
```shell
ag {{foo}} -G {{bar}}
```
#### Znajdź pliki, których zawartość pasuje do wyrażenia regularnego:
```shell
ag '{{^ba(r|z)$}}'
```
#### Znajdź pliki o nazwie pasującej do „foo”:
```shell
ag -g {{foo}}
```
{% endraw %}