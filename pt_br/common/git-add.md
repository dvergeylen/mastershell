---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/pt_br/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adiciona arquivos modificados na área de preparação.
> Mais informações: <https://git-scm.com/docs/git-add>.

#### Adiciona um arquivo na área de preparação:
```shell
git add {{caminho/do/arquivo}}
```
#### Adiciona todos arquivos (rastreados ou não):
```shell
git add -A
```
#### Adiciona apenas arquivos rastreados:
```shell
git add -u
```
#### Adiciona arquivos ignorados:
```shell
git add -f
```
#### Interativamente adiciona partes dos arquivo:
```shell
git add -p
```
#### Interativamente adiciona partes de um dado arquivo:
```shell
git add -p {{caminho/para/arquivo}}
```
#### Interativamente adiciona arquivos ou partes modificadas:
```shell
git add -i
```
{% endraw %}