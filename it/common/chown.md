---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/it/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia utente e gruppo proprietario di file e directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/chown>.

#### Cambia l'utente proprietario di un file/directory:
```shell
chown {{utente}} {{percorso/a/file_o_directory}}
```
#### Cambia utente e gruppo proprietari di un file/directory:
```shell
chown {{utente}}:{{gruppo}} {{percorso/a/file_o_directory}}
```
#### Cambia ricorsivamente il proprietario di una cartella ed i suoi contenuti:
```shell
chown -R {{utente}} {{percorso/alla/directory}}
```
#### Cambia il proprietario di un link simbolico:
```shell
chown -h {{utente}} {{percorso/al/link_simbolico}}
```
#### Cambia il proprietario di un file/directory rendendolo uguale a quello di un altro file di riferimento:
```shell
chown --reference={{percorso/al/file_riferimento}} {{percorso/a/file_o_directory}}
```
{% endraw %}