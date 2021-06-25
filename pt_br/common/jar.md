---
layout: default
title: "jar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jar">
  <a href="/pt_br/common/jar.html">jar</a> <a href="#jar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compactador de Bibliotecas e Aplicações Java.
> Mais informações: <https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

#### Arquiva recursivamente todos os arquivos do diretório atual em um arquivo .jar:
```shell
jar cf {{arquivo.jar}} *
```
#### Descompacta o arquivo .jar/.war para o diretório atual:
```shell
jar -xvf {{arquivo.jar}}
```
#### Lista o conteúdo do arquivo .jar/.war:
```shell
jar tf {{caminho/para/arquivo.jar}}
```
#### Lista o conteúdo do arquivo .jar/.war com mais detalhes (verbose):
```shell
jar tvf {{caminho/para/arquivo.jar}}
```
{% endraw %}