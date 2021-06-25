---
layout: default
title: "aws"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws">
  <a href="/de/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Das offizielle CLI für Amazon Web Services.
> Ausführungssassistent, SSO, Autovervollständigung von Ressourcen sowie YAML Optionen sind nur unter Version v2 verfügbar.
> Weitere Informationen: <https://aws.amazon.com/cli>.

#### Konfiguriere die AWS Kommandozeile:
```shell
aws configure wizard
```
#### Konfiguriere die AWS Kommandozeile mit Hilfe von SSO:
```shell
aws configure sso
```
#### Zeige Hilfe für ein Kommando an:
```shell
aws {{befehl}} help
```
#### Zeige Informationen über die eigene angenomme Identität (häufig benutzt zur Fehlersuche):
```shell
aws sts get-caller-identity
```
#### Liste alle AWS Ressourcen in einer Region mit YAML Formatierung auf:
```shell
aws dynamodb list-tables --region {{us-east-1}} --output yaml
```
#### Erstelle einen IAM Benutzer mit Ausführungsassistent:
```shell
aws iam create-user --cli-auto-prompt
```
#### Öffne einen Assitenten für eine AWS Ressource:
```shell
aws dynamodb wizard {{neue_tabelle}}
```
#### Erstelle einen JSON CLI-Aufbau (hilfreich für Infrastruktur-Automation):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}