---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/pl/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wykonuje polecenia o zadanym czasie.
> Aby działać poprawnie wymaga działającego serwisu atd (lub atrun).
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Wykonaj za 5 minut polecenie wprowadzone przy użyciu wejścia standardowego (aby zakończyć naciśnij `Ctrl + D`):
```shell
at now + 5 minutes
```
#### Wykonaj o 10:00 rano polecenie podane z wejścia standardowego:
```shell
echo "{{./zrób_backup.sh}}" | at 1000
```
#### Wykonaj polecenia z podanego pliku w najbliższy wtorek o 21:30:
```shell
at -f {{ścieżka/do/pliku}} 9:30 PM Tue
```
{% endraw %}