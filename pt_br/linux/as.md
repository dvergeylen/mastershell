---
layout: default
title: "as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="as">
  <a href="/pt_br/linux/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Assembler GNU multiplataforma.
> Seu objetivo inicial é realizar o montagem do arquivo gerado pelo `gcc` para ser utilizado pelo `ld`.

#### Realizar a montagem de um arquivo, o resultado dessa operação será gravado no arquivo a.out:
```shell
as {{arquivo.s}}
```
#### Realizar a montagem de um arquivo, o resultado dessa operação será gravado em um arquivo específico:
```shell
as {{arquivo.s}} -o {{saida.o}}
```
#### Realizar a montagem de um arquivo rapidamente, pois ignora o pré-processamento de comentários e espaços em branco. (Deve ser utilizado apenas em compiladores confiáveis):
```shell
as -f {{arquivo.s}}
```
#### Adiciona um caminho na lista de diretórios onde será realizada a busca por arquivos especificados na diretiva .include:
```shell
as -I {{caminho_para_o_diretorio}} {{arquivo.s}}
```
{% endraw %}