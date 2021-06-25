---
layout: default
title: "git repack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-repack">
  <a href="/it/common/git-repack.html">git repack</a> <a href="#git-repack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comprimi gli oggetti decompressi in un repository Git.
> Maggiori informazioni: <https://git-scm.com/docs/git-repack>.

#### Comprimi gli oggetti decompressi nella cartella corrente:
```shell
git repack
```
#### Rimuovi eventuali archivi ridondanti dopo la compressione:
```shell
git repack -d
```
{% endraw %}