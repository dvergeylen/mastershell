---
layout: default
title: "emacsclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emacsclient">
  <a href="/it/common/emacsclient.html">emacsclient</a> <a href="#emacsclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apri file in un server emacs esistente.
> Maggiori informazioni: <https://www.emacswiki.org/emacs/EmacsClient>.

#### Apri un file in un server Emacs esistene (utilizzando la GUI se disponibile):
```shell
emacsclient {{nome_file}}
```
#### Apri un file in modalità console (senza finestra X):
```shell
emacsclient -nw {{nome_file}}
```
#### Apri un file in un frame Emacs esistente e ritorna immediatamente:
```shell
emacsclient -n {{nome_file}}
```
{% endraw %}