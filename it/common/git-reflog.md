---
layout: default
title: "git reflog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reflog">
  <a href="/it/common/git-reflog.html">git reflog</a> <a href="#git-reflog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra la cronologia delle modifiche a riferimenti locali come HEAD, rami o tag.
> Maggiori informazioni: <https://git-scm.com/docs/git-reflog>.

#### Mostra il reflog di HEAD:
```shell
git reflog
```
#### Mostra il reflog di uno specifico ramo:
```shell
git reflog {{nome_ramo}}
```
#### Mostra le ultime 5 voci del reflog:
```shell
git reflog -n {{5}}
```
{% endraw %}