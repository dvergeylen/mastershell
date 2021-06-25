---
layout: default
title: "gzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gzip">
  <a href="/pt_br/common/gzip.html">gzip</a> <a href="#gzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de compactação de arquivos com compressão gzip.
> Mais informações: <https://www.gnu.org/software/gzip/manual/gzip.html>.

#### Alterar compressão de um arquivo compactado com compressão gzip:
```shell
gzip {{arquivo.ext}}
```
#### Descompactar arquivo gzip definindo arquivo final:
```shell
gzip -c -d {{arquivo.ext}}.gz > {{arquivo_descompactado.ext}}
```
#### Compactar arquivo definindo arquivo final:
```shell
gzip -c {{arquivo.ext}} > {{arquivo_compactado.ext.gz}}
```
#### Compactando arquivos em gzip definindo o nível de compressão [9]:
```shell
gzip -{{9}} -c {{arquivo.ext}} > {{arquivo_compactado.ext.gz}}
```
{% endraw %}