---
layout: default
title: "aws s3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-s3">
  <a href="/pt_br/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interface de linha de comando para AWS S3.
> Provê armazenamento através de uma interface de web services.
> Mais informações: <https://aws.amazon.com/cli>.

#### Exibe arquivos de um bucket:
```shell
aws s3 ls {{nome_do_bucket}}
```
#### Sincroniza arquivos e diretórios locais para o bucket:
```shell
aws s3 sync {{caminho/para/arquivos}} s3://{{nome_do_bucket}}
```
#### Sincroniza arquivos e diretórios do bucket para diretório local:
```shell
aws s3 sync s3://{{nome_do_bucket}} {{caminho/para/diretório}}
```
#### Sincroniza arquivos e diretórios excluindo algo:
```shell
aws s3 sync {{caminho/para/arquivos}} s3://{{nome_do_bucket}} --exclude {{arquivo/não/sincronizado}} --exclude {{caminho/não/sincronizado}}/*
```
#### Remove arquivo do bucket:
```shell
aws s3 rm s3://{{nome_do_bucket}}/{{caminho/do/arquivo}}
```
#### Somente exibe a prévia das mudanças:
```shell
aws s3 {{qualquer_comando}} --dryrun
```
{% endraw %}