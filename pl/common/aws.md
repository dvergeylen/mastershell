---
layout: default
title: "aws"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws">
  <a href="/pl/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Oficjalne narzędzie CLI dla Amazon Web Services.
> Wizard, SSO, Resource Autocompletion, i opcje YAML są tylko v2.
> Więcej informacji: <https://aws.amazon.com/cli>.

#### Konfiguruj AWS Command-line:
```shell
aws configure wizard
```
#### Konfiguruj AWS Command-line używając SSO:
```shell
aws configure sso
```
#### Zobacz tekst pomocy dla polecenia AWS:
```shell
aws {{komenda}} help
```
#### Uzyskaj tożsamość wywołującego (służy do rozwiązywania problemów z uprawnieniami):
```shell
aws sts get-caller-identity
```
#### Wyświetla listę zasobów AWS w regionie i wyświetla w yaml:
```shell
aws dynamodb list-tables --region {{us-east-1}} --output yaml
```
#### Użyj auto prompt do pomocy z poleceniem:
```shell
aws iam create-user --cli-auto-prompt
```
#### Uzyskaj interaktywnego kreatora dla zasobu AWS:
```shell
aws dynamodb wizard {{nowa_tabela}}
```
#### Generuj JSON CLI Skeleton (przydatne dla infrastruktury jako kodu):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}