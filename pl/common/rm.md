---
layout: default
title: "rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rm">
  <a href="/pl/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Usuwa pliki lub foldery.
> Więcej informacji: <https://www.gnu.org/software/coreutils/rm>.

#### Usuń pliki z dowolnej lokalizacji:
```shell
rm {{ścieżka/do/pliku}} {{ścieżka/do/innego/pliku}}
```
#### Rekursywnie usuń folder oraz wszystkie jego podfoldery:
```shell
rm -r {{ścieżka/do/folderu}}
```
#### Wymuś usunięcie folderu, bez pytania o potwierdzenie lub pokazywania błędów:
```shell
rm -rf {{ścieżka/do/folderu}}
```
#### Interaktywnie usuń kilka plików z pytaniem o potwierdzenie przed każdym usunięciem:
```shell
rm -i {{plik(i)}}
```
#### Usuń pliki w trybie opisowym, pokazując wiadomość o każdym usuniętym pliku:
```shell
rm -v {{ścieżka/do/folderu/*}}
```
{% endraw %}