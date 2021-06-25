---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/pt_br/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compactador de arquivos com alta taxa de compressão.
> Versão compacta do `7z`, com suporte para menos tipos de arquivamento/compressão.
> Mais informações: <https://www.7-zip.org/>.

#### Compactar um arquivo ou diretório:
```shell
7za a {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretório}}
```
#### Descompactar um arquivo mantendo a estrutura de diretórios original:
```shell
7za x {{arquivo_compactado.7z}}
```
#### Compactar utilizando um tipo específico de arquivamento/compressão:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretório}}
```
#### Exibir os tipos de arquivamento/compressão disponíveis:
```shell
7za i
```
#### Exibir o conteúdo de um arquivo:
```shell
7za l {{arquivo.7z}}
```
{% endraw %}