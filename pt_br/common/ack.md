---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/pt_br/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uma ferramenta de pesquisa similar ao grep, otimizada para programadores.
> Mais informações: <https://beyondgrep.com/documentation/>.

#### Procurar por arquivos que contenham o termo "foo":
```shell
ack {{foo}}
```
#### Procurar por arquivos em uma linguagem específica:
```shell
ack --ruby {{each_with_object}}
```
#### Contar o número total de correspondências para o termo "foo":
```shell
ack -ch {{foo}}
```
#### Mostrar o nome dos arquivos contendo o termo "foo" e o número de correspondências em cada arquivo:
```shell
ack -cl {{foo}}
```
{% endraw %}