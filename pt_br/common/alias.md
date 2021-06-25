---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/pt_br/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cria apelidos -- palavras que são substituídas por um comando.
> Apelidos expiram ao final da sessão atual do shell de comando, a menos que sejam definidos no arquivo de configuração do shell, por exemplo `~/.bashrc`.
> Mais informações: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Criar um apelido:
```shell
alias {{apelido}}="{{comando}}"
```
#### Visualizar o comando associado a um determinado apelido:
```shell
alias {{apelido}}
```
#### Remover um apelido:
```shell
unalias {{apelido}}
```
#### Exibir todos os apelidos definidos:
```shell
alias -p
```
#### Tornar o comando `rm` interativo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Criar o apelido `la` como um atalho para `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}