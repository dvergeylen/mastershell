---
layout: default
title: "aws s3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-s3">
  <a href="/de/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI für AWS S3. AWS S3 stellt Speicherplatz in der Cloud zur Verfügung.
> Weitere Informationen: <https://aws.amazon.com/cli>.

#### Liste alle Objekte in einem Bucket auf:
```shell
aws s3 ls {{bucket_name}}
```
#### Synchronisiere Dateien und Verzeichnissen zu einem Bucket:
```shell
aws s3 sync {{pfad/zu/datei_oder_verzeichnis}} s3://{{bucket_name}}
```
#### Synchronisiere Dateien und Verzeichnissen von einem Bucket:
```shell
aws s3 sync s3://{{bucket_name}} {{pfad/zu/ziel}}
```
#### Synchronisiere Dateien und Verzeichnissen mit Ausnahmen:
```shell
aws s3 sync {{pfad/zu/datei_oder_verzeichnis}} s3://{{bucket_name}} --exclude {{pfad/zu/datei}} --exclude {{pfad/zu/verzeichnis}}/*
```
#### Entferne ein Objekt von einem Bucket:
```shell
aws s3 rm s3://{{bucket}}/{{pfad/zu/datei}}
```
#### Probelauf eines angegeben Kommandos ohne diesen auszuführen:
```shell
aws s3 {{befehl}} --dryrun
```
{% endraw %}