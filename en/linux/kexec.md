---
layout: default
title: "kexec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kexec">
  <a href="/en/linux/kexec.html">kexec</a> <a href="#kexec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Directly reboot into a new kernel.

#### Load a new kernel:
```shell
kexec -l {{path/to/kernel}} --initrd={{path/to/initrd}} --command-line={{arguments}}
```
#### Load a new kernel with current boot parameters:
```shell
kexec -l {{path/to/kernel}} --initrd={{path/to/initrd}} --reuse-cmdline
```
#### Execute a currently loaded kernel:
```shell
kexec -e
```
#### Unload current kexec target kernel:
```shell
kexec -u
```
{% endraw %}