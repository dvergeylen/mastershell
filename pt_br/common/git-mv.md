---
layout: default
title: "git mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mv">
  <a href="/pt_br/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move ou renomeia arquivos e atualiza o index do Git.
> Mais informações: <https://git-scm.com/docs/git-mv>.

#### Move arquivos dentro de um repositório e adiciona no próximo commit:
```shell
git mv {{caminho/para/arquivo}} {{novo/caminho}}
```
#### Renomeia um arquivo e adiciona a renomeação no próximo commit:
```shell
git mv {{nome_do_arquivo}} {{novo_nome}}
```
#### Sobrescreve o arquivo no caminho alvo se ele já existir:
```shell
git mv --force {{arquivo}} {{alvo}}
```
{% endraw %}