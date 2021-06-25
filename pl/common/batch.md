---
layout: default
title: "batch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="batch">
  <a href="/pl/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wykonaj polecenia, gdy pozwoli na to poziom obciążenia systmu.
> Aby działać poprawnie wymaga działającego serwisu atd (lub atrun).
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Wykonaj polecenie wprowadzone przy użyciu wejścia standardowego (aby zakończyć naciśnij `Ctrl + D`):
```shell
batch
```
#### Wykonaj polecenie podane z wejścia standardowego:
```shell
echo "{{./zrób_backup.sh}}" | batch
```
#### Wykonaj polecenia z podanego pliku:
```shell
batch -f {{ścieżka/do/pliku}}
```
{% endraw %}