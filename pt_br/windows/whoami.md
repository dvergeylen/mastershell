---
layout: default
title: "whoami"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whoami">
  <a href="/pt_br/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra detalhes sobre o usuário atual.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/whoami>.

#### Mostra o username do usuário atual:
```shell
whoami
```
#### Mostra os grupos dos quais o usuário atual faz parte:
```shell
whoami /groups
```
#### Mostra os privilégios do usuário atual:
```shell
whoami /priv
```
#### Mostra o nome principal (UPN) do usuário atual:
```shell
whoami /upn
```
#### Mostra o id de logon do usuário atual:
```shell
whoami /logonid
```
{% endraw %}