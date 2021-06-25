---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/pt_br/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um compactador de arquivos com alta taxa de compressão.
> Versão do `7z` com suporte apenas para o formato `.7z`.
> Mais informações: <https://www.7-zip.org/>.

#### Compactar um arquivo ou diretório:
```shell
7zr a {{arquivo_compactado.7z}} {{caminho/arquivo_ou_diretorio}}
```
#### Descompactar um arquivo mantendo a estrutura de diretórios original:
```shell
7zr x {{arquivo_compactado.7z}}
```
#### Exibir o conteúdo de um arquivo:
```shell
7zr l {{arquivo_compactado.7z}}
```
{% endraw %}