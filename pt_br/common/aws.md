---
layout: default
title: "aws"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws">
  <a href="/pt_br/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A interface de linha de comando oficial para o Amazon Web Services.
> Passo-a-passo, Single Sign-On (SSO), autocompletar de recursos e opções de YAML somente na v2.
> Mais informações: <https://aws.amazon.com/cli>.

#### Configura a linha de comando da AWS:
```shell
aws configure wizard
```
#### Configura a linha de comando da AWS usando o SSO:
```shell
aws configure sso
```
#### Veja o texto de ajuda para o comando da AWS:
```shell
aws {{comando}} help
```
#### Obtenha a informações da identidade usada (útil para analisar problemas de permissão):
```shell
aws sts get-caller-identity
```
#### Lista recursos da AWS em uma região em yaml:
```shell
aws dynamodb list-tables --region {{sa-east-1}} --output yaml
```
#### Usa prompt de comando para ajuda com o preenchimento:
```shell
aws iam create-user --cli-auto-prompt
```
#### Usa um passo-a-passo interativo para um recurso da AWS:
```shell
aws dynamodb wizard {{nova-tabela}}
```
#### Gera um arquivo esqueleo em JSON (útil para ser usado em infraestrutura como código):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}