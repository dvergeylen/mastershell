---
layout: default
title: "tar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tar">
  <a href="/pt_br/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de compressão de arquivos.
> Utilizado com metodos de compressão como o de gzip ou bzip2.
> Mais informações: <https://www.gnu.org/software/tar>.

#### Compactando arquivos em um arquivo tar:
```shell
tar -cvf {{output.tar}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Compactando arquivos em arquivo gzip:
```shell
tar -czvf {{output.tar.gz}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Compactando arquivos definindo tipo de compressão automaticamente por extensão:
```shell
tar -cavf {{output.tar.xz}} {{arquivo1}} {{arquivo2}} {{arquivo3}}
```
#### Extraindo arquivos de um arquivo compactado:
```shell
tar -xvf {{input.tar[.gz|.bz2|.xz]}}
```
#### Extraindo arquivos de um arquivo compactado filtrando por gzip:
```shell
tar -xzvf {{input.tar[.gz|.bz2|.xz]}}
```
#### Extraindo arquivos de um arquivo compactado para um diretório específico:
```shell
tar -xvf {{input.tar[.gz|.bz2|.xz]}} -C {{diretório}}
```
#### Extrair arquivos seguindo um padrão:
```shell
tar -xvf {{input.tar}} --wildcards "{{*.html}}"
```
#### Listando arquivos de um arquivo tar:
```shell
tar -tvf {{input.tar}}
```
{% endraw %}