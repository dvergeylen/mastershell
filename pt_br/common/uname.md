---
layout: default
title: "uname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uname">
  <a href="/pt_br/common/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apresenta detalhes sobre o hardware e sistema operacional do computador.
> Nota: Para maiores detalhes sobre o sistema operacional, utilize o comando `lsb_release`.
> Mais informações: <https://www.gnu.org/software/coreutils/uname>.

#### Exibir informações relacionadas ao hardware: arquitetura e tipo de processador:
```shell
uname -mp
```
#### Exibir informações relacionadas ao software: sistema operacional, número da release e versão:
```shell
uname -srv
```
#### Exibir o nome de rede do computador:
```shell
uname -n
```
#### Exibir todas as informações disponíveis do sistema (hardware, software, nome de rede):
```shell
uname -a
```
{% endraw %}