---
layout: default
title: "git blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-blame">
  <a href="/it/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra hash del commit ed ultimo autore per ogni riga di un file.
> Maggiori informazioni: <https://git-scm.com/docs/git-blame>.

#### Stampa il contenuto di un file annotando ogni riga con l'hash del commit e il nome dell'autore:
```shell
git blame {{file}}
```
#### Stampa il contenuto di un file annotando ogni riga con l'hash del commit e l'indirizzo email dell'autore:
```shell
git blame -e {{file}}
```
{% endraw %}