---
layout: default
title: "gdb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gdb">
  <a href="/en/common/gdb.html">gdb</a> <a href="#gdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The GNU Debugger.
> More information: <https://www.gnu.org/software/gdb>.

#### Debug an executable:
```shell
gdb {{executable}}
```
#### Attach a process to gdb:
```shell
gdb -p {{procID}}
```
#### Debug with a core file:
```shell
gdb -c {{core}} {{executable}}
```
#### Execute given GDB commands upon start:
```shell
gdb -ex "{{commands}}" {{executable}}
```
#### Start gdb and pass arguments to the executable:
```shell
gdb --args {{executable}} {{argument1}} {{argument2}}
```
{% endraw %}