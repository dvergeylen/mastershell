---
layout: default
title: "pathchk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pathchk">
  <a href="/pl/common/pathchk.html">pathchk</a> <a href="#pathchk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sprawdź poprawność oraz przenośność jednej lub większej ilości ścieżek.
> Więcej informacji: <https://www.gnu.org/software/coreutils/pathchk>.

#### Sprawdź ścieżki pod kątem poprawności w obecnym systemie:
```shell
pathchk {{ścieżka1 ścieżka2 …}}
```
#### Sprawdź ścieżki pod kątem poprawności w szerszym zakresie systemów zgodnych z POSIX:
```shell
pathchk -p {{ścieżka1 ścieżka2 …}}
```
#### Sprawdź ścieżki pod kątem poprawności we wszystkich systemach zgodnych z POSIX:
```shell
pathchk --portability {{ścieżka1 ścieżka2 …}}
```
#### Sprawdź tylko pod kątem pustych ścieżek lub wiodących myślników (-):
```shell
pathchk -P {{ścieżka1 ścieżka2 …}}
```
{% endraw %}