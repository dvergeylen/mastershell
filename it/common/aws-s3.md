---
layout: default
title: "aws s3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-s3">
  <a href="/it/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI per AWS S3 - fornisce spazio di archiviazione tramite le interfacce di Amazon Web Services.
> Maggiori informazioni: <https://aws.amazon.com/cli>.

#### Mostra file in un bucket:
```shell
aws s3 ls {{nome_bucket}}
```
#### Sincronizza file e directory locali su un bucket:
```shell
aws s3 sync {{percorso/ai/file}} s3://{{nome_bucket}}
```
#### Sincronizza file e directory da un bucket in locle:
```shell
aws s3 sync s3://{{nome_bucket}} {{path/to/target}}
```
#### Sincronizza file e directory escludendo alcuni file o directory:
```shell
aws s3 sync {{percorso/ai/file}} s3://{{nome_bucket}} --exclude {{percorso/al/file}} --exclude {{directory}}/*
```
#### Rimuovi un file dal bucket:
```shell
aws s3 rm s3://{{bucket}}/{{percorso/al/file}}
```
#### Mostra solo un'anteprima dei cambiamenti:
```shell
aws s3 {{qualsiasi_comando}} --dryrun
```
{% endraw %}