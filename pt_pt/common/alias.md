---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/pt_pt/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cria um alias -- palavras que são substituídas por um comando.
> Alias expiram com a sessão da shell atual, a menos que sejam definidos no ficheiro de configuração da shell, por exemplo `~/.bashrc`.
> Mais informações: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Listar todos os alias:
```shell
alias
```
#### Criar um alias genérico:
```shell
alias {{palavra}}="{{comando}}"
```
#### Visualizar o comando associado a um dado alias:
```shell
alias {{palavra}}
```
#### Remover um alias de um comando:
```shell
unalias {{palavra}}
```
#### Tornar `rm` num comando interativo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Criar `la` como um atalho para `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}