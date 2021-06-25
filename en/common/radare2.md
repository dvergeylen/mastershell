---
layout: default
title: "radare2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="radare2">
  <a href="/en/common/radare2.html">radare2</a> <a href="#radare2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A set of reverse engineering tools.
> More information: <https://radare.gitbooks.io/radare2book/>.

#### Open a file in write mode without parsing the file format headers:
```shell
radare2 -nw {{path/to/binary}}
```
#### Debug a program:
```shell
radare2 -d {{path/to/binary}}
```
#### Run a script before entering the interactive CLI:
```shell
radare2 -i {{path/to/script.r2}} {{path/to/binary}}
```
#### Show help text for any command in the interactive CLI:
```shell
> {{radare2_command}}?
```
#### Run a shell command from the interactive CLI:
```shell
> !{{shell_command}}
```
#### Dump raw bytes of current block to a file:
```shell
> pr > {{path/to/file.bin}}
```
{% endraw %}