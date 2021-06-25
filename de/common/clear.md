---
layout: default
title: "clear"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clear">
  <a href="/de/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Leert den Bildschirm eines Terminals.
> Weitere Informationen: <https://manned.org/clear>.

#### Leere den Bildschirm (äquivalent zu Strg+L in einer Bash Shell):
```shell
clear
```
#### Leere den Bildschirm, aber erhalte den Rückscroll-Puffer des Terminals:
```shell
clear -x
```
#### Lege den Typ des zu leerenden Terminals fest (Standardwert ist die Umgebungsvariable $TERM):
```shell
clear -T {{typ_des_terminals}}
```
#### Zeige die Version von `ncurses` an, die von `clear` benutzt wird:
```shell
clear -V
```
{% endraw %}