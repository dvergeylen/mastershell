---
layout: default
title: "git pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pull">
  <a href="/it/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scarica oggetti e riferimenti (fetch) da un repository remoto e avvia un'unione (merge) con il ramo corrente.
> Maggiori informazioni: <https://git-scm.com/docs/git-pull>.

#### Scarica le ultime modifiche dal repository remoto e avvia un'unione:
```shell
git pull
```
#### Scarica le ultime modifiche dal repository remoto e avvia un rebase:
```shell
git pull --rebase
```
#### Scarica le ultime modifiche da uno specifico ramo remoto e avvia un'unione con il ramo corrente:
```shell
git pull {{nome_repository_remoto}} {{nome_ramo}}
```
{% endraw %}