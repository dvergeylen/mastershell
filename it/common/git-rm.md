---
layout: default
title: "git rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rm">
  <a href="/it/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cancella file dall'indice del repository e dal filesystem locale.
> Maggiori informazioni: <https://git-scm.com/docs/git-rm>.

#### Cancella un file dall'indice del repository e dal filesystem:
```shell
git rm {{file}}
```
#### Cancella una cartella:
```shell
git rm -r {{cartella}}
```
#### Cancella un file dall'indice del repository ma non dal filesystem locale:
```shell
git rm --cached {{file}}
```
{% endraw %}