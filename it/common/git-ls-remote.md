---
layout: default
title: "git ls-remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-remote">
  <a href="/it/common/git-ls-remote.html">git ls-remote</a> <a href="#git-ls-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elenca i riferimenti in un repository remoto dato un nome o un URL.
> Qualora né nome né URL siano specificati, il ramo predefinito è upstream - se configurato - oppure origin.
> Maggiori informazioni: <https://git-scm.com/docs/git-ls-remote>.

#### Mostra tutti i riferimenti nel repository remoto predefinito:
```shell
git ls-remote
```
#### Mostra solo i riferimenti HEAD nel repository remoto predefinito:
```shell
git ls-remote --heads
```
#### Mostra solo i riferimenti a tag nel repository remoto predefinito:
```shell
git ls-remote --tags
```
#### Mostra tutti i riferimenti da un repository remoto dato un nome o URL:
```shell
git ls-remote {{url_repository}}
```
#### Filtra i riferimenti da un repository remoto rispetto a un dato criterio:
```shell
git ls-remote {{nome_repository}} "{{criterio}}"
```
{% endraw %}