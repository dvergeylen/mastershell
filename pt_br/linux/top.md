---
layout: default
title: "top"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="top">
  <a href="/pt_br/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário para exibir informações, em tempo real, sobre os processos em execução.

#### Iniciar top:
```shell
top
```
#### Exibir apenas os processos ativos:
```shell
top -i
```
#### Exibir os processos de um usuário específico:
```shell
top -u {{username}}
```
#### Exibir o(s) processo(s) de um ou mais PID específico(s), separado(s) por vírgula:
```shell
top -p {{PID1,PID2,PID3}}
```
#### Mostra Ajuda sobre os comandos disponíveis:
```shell
?
```
{% endraw %}