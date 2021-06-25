---
layout: default
title: "axel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="axel">
  <a href="/pt_br/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Acelerador de downloads.
> Suporta HTTP, HTTPS, e FTP.
> Mais informações: <https://github.com/axel-download-accelerator/axel>.

#### Fazer download de uma URL para um arquivo:
```shell
axel {{url}}
```
#### Fazer download especificando o nome do arquivo de destino:
```shell
axel {{url}} -o {{nome_do_arquivo}}
```
#### Fazer download usando múltiplas conexões:
```shell
axel -n {{número_de_conexões}} {{url}}
```
#### Procurar por mirrors:
```shell
axel -S {{número_de_mirrors}} {{url}}
```
#### Limitar velocidade de download (em bytes por segundo):
```shell
axel -s {{velocidade}} {{url}}
```
{% endraw %}