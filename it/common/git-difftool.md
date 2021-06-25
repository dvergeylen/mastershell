---
layout: default
title: "git difftool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-difftool">
  <a href="/it/common/git-difftool.html">git difftool</a> <a href="#git-difftool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra le modifiche ai file tracciati usando uno strumento Diff esterno. Accetta le stesse opzioni e argomenti di Git diff.
> Maggiori informazioni: <https://git-scm.com/docs/git-difftool>.

#### Elenca gli strumenti Diff disponibili:
```shell
git difftool --tool-help
```
#### Imposta meld come strumento Diff predefinito:
```shell
git config --global diff.tool "{{meld}}"
```
#### Usa lo strumento Diff predefinito per mostrare le modifiche nell'area di stage:
```shell
git difftool --staged
```
#### Uso uno specifico strumento Diff (opendiff) per mostrare le modifiche a partire da un dato commit:
```shell
git difftool --tool={{opendiff}} {{commit}}
```
{% endraw %}