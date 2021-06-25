---
layout: default
title: "git check-ignore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-check-ignore">
  <a href="/it/common/git-check-ignore.html">git check-ignore</a> <a href="#git-check-ignore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analizza ed esegui il debug di ".gitignore" e dei file esclusi.
> Maggiori informazioni: <https://git-scm.com/docs/git-check-ignore>.

#### Verifica se un file o una cartella sono ignorati:
```shell
git check-ignore {{percorso/al/file_o_cartella}}
```
#### Verifica se più file o cartelle sono ignorati:
```shell
git check-ignore {{percorso/al/file}} {{percorso/alla/cartella}}
```
#### Leggi i percorsi di file o cartelle da stdin (uno per riga) invece che dalla riga di comando:
```shell
git check-ignore --stdin < {{percorso/alla/lista_dei_file_o_cartelle}}
```
#### Non controllare nell'indice (usato per determinare il motivo per cui alcuni percorsi non sono ignorati):
```shell
git check-ignore --no-index {{percorsi/ai/file_o_cartelle}}
```
#### Includi dettagli sul pattern corrispondente per ogni percorso specificato:
```shell
git check-ignore --verbose {{percorsi/ai/file_o_cartelle}}
```
{% endraw %}