---
layout: default
title: "print"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="print">
  <a href="/en/windows/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print a text file to a printer.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/print>.

#### Print a text file to the default printer:
```shell
print {{path/to/file}}
```
#### Print a text file to a specific printer:
```shell
print /d:{{printer}} {{path/to/file}}
```
{% endraw %}