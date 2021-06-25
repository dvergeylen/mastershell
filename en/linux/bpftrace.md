---
layout: default
title: "bpftrace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bpftrace">
  <a href="/en/linux/bpftrace.html">bpftrace</a> <a href="#bpftrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> High-level tracing language for Linux eBPF.
> More information: <https://github.com/iovisor/bpftrace>.

#### Display bpftrace version:
```shell
bpftrace -V
```
#### List all available probes:
```shell
sudo bpftrace -l
```
#### Run a one-liner program (e.g syscall count by program):
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter { @[comm] = count(); }}}'
```
#### Run a program from a file:
```shell
sudo bpftrace {{path/to/file}}
```
#### Trace a program by PID:
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter /pid == 123/ { @[comm] = count(); }}}'
```
#### Do a dry run and display the output in eBPF format:
```shell
sudo bpftrace -d -e '{{one_line_program}}'
```
{% endraw %}