---
layout: default
title: "git am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-am">
  <a href="/it/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Applica file di patch. Utile quando si ricevono commit via email.
> Vedi anche `git format-patch` per generare file di patch.
> Maggiori informazioni: <https://git-scm.com/docs/git-am>.

#### Applica un file di patch:
```shell
git am {{percorso/al/file.patch}}
```
#### Interrompi l'applicazione di un file di patch:
```shell
git am --abort
```
#### Applica quanto possibile di un file di patch, salvando le parti non applicabili in file `.rej`:
```shell
git am --reject {{percorso/al/file.patch}}
```
{% endraw %}