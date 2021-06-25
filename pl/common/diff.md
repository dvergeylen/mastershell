---
layout: default
title: "diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diff">
  <a href="/pl/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Porównaj pliki i foldery.

#### Porównaj pliki (lista zmian między `stary_plik` a `nowy_plik`):
```shell
diff {{stary_plik}} {{nowy_plik}}
```
#### Porównaj pliki, ignoruj białe znaki (white spaces):
```shell
diff -w {{stary_plik}} {{nowy_plik}}
```
#### Porównaj pliki, pokaż różnice obok siebie:
```shell
diff -y {{stary_plik}} {{nowy_plik}}
```
#### Porównaj pliki, pokaż różnice w ujednoliconym formacie (tak jak w przypadku `git diff`):
```shell
diff -u {{stary_plik}} {{nowy_plik}}
```
#### Porównaj foldery rekurencyjnie (pokazuje nazwy różniących się plików/folderów a także zmiany w plikach):
```shell
diff -r {{stary_folder}} {{nowy_folder}}
```
#### Porównaj foldery rekurencyjnie, pokaż tylko nazwy plików które się różnią:
```shell
diff -rq {{stary_folder}} {{nowy_folder}}
```
{% endraw %}