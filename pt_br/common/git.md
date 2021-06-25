---
layout: default
title: "git"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git">
  <a href="/pt_br/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sistema de versionamento distribuído.
> Mais informações: <https://git-scm.com>.

#### Verifique a versão do Git:
```shell
git --version
```
#### Mostre ajuda geral:
```shell
git --help
```
#### Mostre ajuda de um subcomando do Git (como `commit`, `log`, etc.):
```shell
git help {{subcomando}}
```
#### Execute um subcomando Git:
```shell
git {{subcomando}}
```
#### Execute um subcomando Git no caminho raíz de um repositório específico:
```shell
git -C {{caminho/para/repo}} {{subcomando}}
```
#### Execute um subcomando Git com uma dada configuração:
```shell
git -c '{{config.chave}}={{valor}}' {{subcomando}}
```
{% endraw %}