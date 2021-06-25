---
layout: default
title: "aws ec2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-ec2">
  <a href="/pt_br/common/aws-ec2.html">aws ec2</a> <a href="#aws-ec2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inteface de linha de comando para o AWS EC2.
> Provê capacidade computacional segura e flexível na nuvem da AWS para proporcionar um desenvolvimento e subida para produção de aplicações rapidamente.
> Mais informações: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html>.

#### Lista todos os comandos EC2 disponíveis:
```shell
aws ec2 help
```
#### Exibe ajuda específica para um subcomando da EC2:
```shell
aws ec2 {{subcomando}} help
```
#### Exibe informações sobre uma insntância específica:
```shell
aws ec2 describe-instances --instance-ids {{id_da_instância}}
```
#### Exibe informações sobre todas as instâncias:
```shell
aws ec2 describe-instances
```
#### Exibe informações sobre todos os volumes EC2:
```shell
aws ec2 describe-volumes
```
#### Deleta um volume EC2:
```shell
aws ec2 delete-volume --volume-id {{id_do_volume}}
```
#### Cria um snapshot de um volume EC2:
```shell
aws ec2 create-snapshot --volume-id {{id_do_volume}}
```
#### Lista as AMIs (Imagem de Máquina da Amazon) disponíveis:
```shell
aws ec2 describe-images
```
{% endraw %}