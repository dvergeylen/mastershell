---
layout: default
title: "aws ec2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-ec2">
  <a href="/de/common/aws-ec2.html">aws ec2</a> <a href="#aws-ec2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI für AWS EC2.
> AWS EC2 stellt eine sichere und skalierbare Einheit in der AWS Cloud zur Verfügung um ein schnelleres Entwickeln und Ausrollen von Software zu ermöglichen.
> Weitere Informationen: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html>.

#### Liste alle verfügbaren EC2 Befehle auf:
```shell
aws ec2 help
```
#### Zeige Hilfe für bestimmte EC2 Unterbefehle an:
```shell
aws ec2 {{unterbefehl}} help
```
#### Liste Informationen zu einer bestimmten Instanz auf:
```shell
aws ec2 describe-instances --instance-ids {{instanz_id}}
```
#### Liste Informationen zu allen Instanzen auf:
```shell
aws ec2 describe-instances
```
#### Liste Informationen zu allen EC2 Volumen auf:
```shell
aws ec2 describe-volumes
```
#### Liste Informationen zu einem bestimmten EC2 Volumen auf:
```shell
aws ec2 describe-volume --volume-id {{volumen_id}}
```
#### Erstelle einen Snapshot, basierend auf einem EC2 Volumen:
```shell
aws ec2 create-snapshot --volume-id {{volumen_id}}
```
#### Liste alle verfügbaren AMIs (Amazon Machine Images) auf:
```shell
aws ec2 describe-images
```
{% endraw %}