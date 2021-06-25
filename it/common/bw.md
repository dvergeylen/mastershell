---
layout: default
title: "bw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bw">
  <a href="/it/common/bw.html">bw</a> <a href="#bw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI per accedere e gestire vault Bitwarden.
> Maggiori informazioni: <https://help.bitwarden.com/article/cli/>.

#### Esegui il login ad un account Bitwarden:
```shell
bw login
```
#### Esegui il logout da un account Bitwarden:
```shell
bw logout
```
#### Cerca e mostra oggetti in un vault Bitwarden:
```shell
bw list items --search {{github}}
```
#### Mostra un particolare oggetto contenuto in un vault Bitwarden:
```shell
bw get item {{github}}
```
#### Crea una cartella in un vault bitwarden:
```shell
{{echo -n '{"name":"Nome cartella"}' | base64}} | bw create folder
```
{% endraw %}