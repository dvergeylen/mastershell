---
layout: default
title: "emacs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emacs">
  <a href="/it/common/emacs.html">emacs</a> <a href="#emacs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Editor di testo in tempo reale, estendibile, personalizzabile e auto documentato.
> Maggiori informazioni: <https://www.gnu.org/software/emacs>.

#### Avvia emacs in modalità console (senza finestra X):
```shell
emacs -nw
```
#### Apri un file in emacs:
```shell
emacs {{nome_file}}
```
#### Esci da emacs (salva i buffer e termina):
```shell
Ctrl + X, Ctrl + C
```
{% endraw %}