---
layout: default
title: "git describe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-describe">
  <a href="/it/common/git-describe.html">git describe</a> <a href="#git-describe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rendi il nome di un oggetto Git più leggibile usando i riferimenti disponibili.
> Maggiori informazioni: <https://git-scm.com/docs/git-describe>.

#### Crea un nome univoco per il commit corrente (il nome contiene i tag più recenti, il numero di commit aggiuntivi, e l'hash breve del commit):
```shell
git describe
```
#### Crea un nome di 4 cifre per l'hash breve del commit:
```shell
git describe --abbrev={{4}}
```
#### Genera un nome che includa anche il percorso di riferimento:
```shell
git describe --all
```
#### Descrivi un tag Git:
```shell
git describe {{v1.0.0}}
```
#### Crea un nome per l'ultimo commit di un dato ramo:
```shell
git describe {{nome_ramo}}
```
{% endraw %}