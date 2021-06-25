---
layout: default
title: "print"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="print">
  <a href="/pt_br/windows/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprimir um arquivo de texto em uma impressora.
> Mais informações: <https://docs.microsoft.com/pt-br/windows-server/administration/windows-commands/print>.

#### Imprimir um arquivo de texto na impressora padrão:
```shell
print {{caminho/para/arquivo}}
```
#### Imprimir arquivo de texto em uma impressora específica:
```shell
print /d:{{impressora}} {{caminho/para/arquivo}}
```
{% endraw %}