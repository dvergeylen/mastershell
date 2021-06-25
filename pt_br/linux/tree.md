---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/pt_br/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibe o conteúdo do diretório atual em formato de árvore.
> Mais informações: <https://guialinux.uniriotec.br/tree/>.

#### Exibe os arquivos e diretórios de acordo com o nível de profundidade 'num' informado (onde 1 significa o diretório atual):
```shell
tree -L {{num}}
```
#### Exibe apenas diretórios:
```shell
tree -d
```
#### Inclui a exibição de arquivos ocultos com colorização diferenciada:
```shell
tree -a -C
```
#### Exibe a árvore sem identação, mostrando o caminho completo (usar `-N` para não escapar espaços em branco e caracteres especiais):
```shell
tree -i -f
```
#### Exibe o tamanho de cada arquivo e o tamanho acumulado de cada diretório, em um formato de leitura para humanos:
```shell
tree -s -h --du
```
#### Exibe arquivos em uma árvore hierárquica, utilizando um padrão coringa, e eliminando diretórios que não contêm arquivos correspondentes ao informado:
```shell
tree -P '{{*.txt}}' --prune
```
#### Exibe diretórios em uma árvore hierárquica, utilizando um padrão coringa, e eliminando diretórios que não possuem ancestrais do informado:
```shell
tree -P {{nome_diretorio}} --matchdirs --prune
```
#### Exibe a árvore ignorando os diretórios informados:
```shell
tree -I '{{nome_diretorio1|nome_diretorio2}}'
```
{% endraw %}