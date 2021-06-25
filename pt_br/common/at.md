---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/pt_br/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta para o agendamento de comandos.
> O serviço atd (ou atrun) deve estar sendo executado para as atuais execuções.
> Mais informações: <https://man.archlinux.org/man/at.1>.

#### Executar comandos da standard input em 5 minutos (pressionar `Ctrl + D`quando acabar):
```shell
at now + {{5}} minutes
```
#### Executar um comando da standard input às 10:00 da manhã de hoje:
```shell
echo "{{./comando.sh}}" | at 1000
```
#### Executar comandos de um dado arquivo na próxima terça:
```shell
at -f {{caminho/para/arquivo}} 9:30 PM Tue
```
{% endraw %}