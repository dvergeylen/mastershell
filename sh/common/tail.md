---
layout: default
title: "tail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tail">
  <a href="/sh/common/tail.html">tail</a> <a href="#tail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prikazuje krajnji deo datoteke.
> Više informacija: <https://www.gnu.org/software/coreutils/tail>.

#### Prikaži poslednjih 'broj' linija u datoteci:
```shell
tail -n {{broj}} {{datoteka}}
```
#### Prikaži celu datoteku od linije 'broj':
```shell
tail -n +{{broj}} {{datoteka}}
```
#### Prikaži poslednjih 'broj' bajtova u datoteci:
```shell
tail -c {{broj}} {{datoteka}}
```
#### Čitaj datoteku sve do `Ctrl + C`:
```shell
tail -f {{datoteka}}
```
#### Čitaj datoteku sve do `Ctrl + C`, čak i kad je datoteka rotirana:
```shell
tail -F {{datoteka}}
```
{% endraw %}