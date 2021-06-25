---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/pt_br/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerencia repositórios monitorados ("remotes").
> Mais informações: <https://git-scm.com/docs/git-remote>.

#### Mostre uma lista de remotes existentes, seus nomes e URL:
```shell
git remote -v
```
#### Mostra infomação de um remote específico:
```shell
git remote show {{nome_do_remote}}
```
#### Adiciona um remote:
```shell
git remote add {{nome_do_remote}} {{url_do_remote}}
```
#### Muda a URL de um remote (use `--add` para manter a URL existente):
```shell
git remote set-url {{nome_do_remote}} {{nova_url}}
```
#### Remove um remote:
```shell
git remote remove {{nome_do_remote}}
```
#### Renomeia um remote:
```shell
git remote rename {{nome_antigo}} {{novo_nome}}
```
{% endraw %}