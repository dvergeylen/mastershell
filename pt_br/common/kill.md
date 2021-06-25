---
layout: default
title: "kill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kill">
  <a href="/pt_br/common/kill.html">kill</a> <a href="#kill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Envia um sinal para um processo, geralmente para finalizar o processo.
> Todos os sinais exceto pelo SIGKILL e SIGSTOP podem ser interceptados pelo processo para finalizar de forma limpa.

#### Finaliza um programa usando o sinal default SIGTERM (terminate):
```shell
kill {{id_do_processo}}
```
#### Lista todos os nomes dos sinais disponíveis (para serem usados sem o prefixo `SIG`):
```shell
kill -l
```
#### Finaliza um processo em background:
```shell
kill %{{id_do_processo}}
```
#### Finaliza um programa usando o sinal SIGHUP. Muitos daemons vão recarregar ao invés de finalizar:
```shell
kill -{{1|HUP}} {{id_do_processo}}
```
#### Finaliza um programa usando o sinal SIGINT (interrupt). Isto é tipicamente iniciado pelo usuário ao pressionar `Ctrl + C`:
```shell
kill -{{2|INT}} {{id_do_processo}}
```
#### Envia sinal para o sistema operacional para finalizar imediatamente o programa (quem não tem chance de capturar o sinal):
```shell
kill -{{9|KILL}} {{id_do_processo}}
```
#### Envia sinal para o sistema operacional para pausar o programa até um sinal SIGCONT ("continue") seja recebido:
```shell
kill -{{17|STOP}} {{id_do_processo}}
```
#### Envia um sinal `SIGUSR1` para todos os processos de um dado GID (group id):
```shell
kill -{{SIGUSR1}} -{{id_do_grupo}}
```
{% endraw %}