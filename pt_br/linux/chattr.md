---
layout: default
title: "chattr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chattr">
  <a href="/pt_br/linux/chattr.html">chattr</a> <a href="#chattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Altera os atributos de arquivos ou diretórios.

#### Bloquear um arquivo ou diretório para mudanças ou remoção, mesmo para um super usuário:
```shell
chattr +i {{caminho_do_arquivo_ou_diretorio}}
```
#### Desbloquear um arquivo ou diretório:
```shell
chattr -i {{caminho_do_arquivo_ou_diretorio}}
```
#### Bloquear diretório e todos os seus arquivos para mudanças ou remoção:
```shell
chattr -R +i {{caminho_do_diretorio}}
```
{% endraw %}