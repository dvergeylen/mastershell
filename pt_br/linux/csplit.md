---
layout: default
title: "csplit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csplit">
  <a href="/pt_br/linux/csplit.html">csplit</a> <a href="#csplit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Divide um arquivo em várias partes.
> O padrão de nomenclatura dos arquivos será "xx00", "xx01" e assim por diante.
> Mais informações: <https://www.gnu.org/software/coreutils/csplit>.

#### Dividir um arquivo nas linhas 5 e 23:
```shell
csplit {{arquivo}} {{5}} {{23}}
```
#### Dividir um arquivo a cada 5 linhas (este comando irá falhar se o total de linhas do arquivo não for divisível por 5):
```shell
csplit {{arquivo}} {{5}} {*}
```
#### Dividir um arquivo a cada 5 linhas, ignorando o fato do total de linhas ser divisível por 5:
```shell
csplit -k {{arquivo}} {{5}} {*}
```
#### Dividir o arquivo na linha 5 e utilizar um prefixo específico para os arquivos de saída:
```shell
csplit {{arquivo}} {{5}} -f {{prefix}}
```
#### Dividir um arquivo na linha que atenda a expressão regular:
```shell
csplit {{arquivo}} /{{expressao_regular}}/
```
{% endraw %}