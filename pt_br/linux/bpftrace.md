---
layout: default
title: "bpftrace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bpftrace">
  <a href="/pt_br/linux/bpftrace.html">bpftrace</a> <a href="#bpftrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Linguagem de análise de alto nível para eBPF Linux.
> Mais informações: <https://github.com/iovisor/bpftrace>.

#### Verifique a versão do bpftrace:
```shell
bpftrace -V
```
#### Lista todos os probes:
```shell
sudo bpftrace -l
```
#### Rode um programa de uma linha (e.g. número de syscalls por programa):
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter { @[comm] = count(); }}}'
```
#### Rode um programa de um arquivo:
```shell
sudo bpftrace {{caminho/do/arquivo}}
```
#### Analise um programa por PID:
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter /pid == 123/ { @[comm] = count(); }}}'
```
#### Mostre o resultado do programa em eBPF, sem rodar ele:
```shell
sudo bpftrace -d -e '{{programa_de_uma_linha}}'
```
{% endraw %}