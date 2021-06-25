---
layout: default
title: "choco info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-info">
  <a href="/pt_br/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibir informações detalhadas de um pacote com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-info>.

#### Exibir informações sobre um pacote específico:
```shell
choco info {{pacote}}
```
#### Exibir informação para um pacote local:
```shell
choco info {{pacote}} --local-only
```
#### Especificar uma fonte personalizada para receber as informações de um pacote:
```shell
choco info {{pacote}} --source {{url_da_fonte|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco info {{pacote}} --user {{apelido}} --password {{senha}}
```
{% endraw %}