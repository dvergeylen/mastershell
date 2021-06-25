---
layout: default
title: "aws s3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-s3">
  <a href="/en/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for AWS S3 - provides storage through web services interfaces.
> More information: <https://aws.amazon.com/cli>.

#### Show files in a bucket:
```shell
aws s3 ls {{bucket_name}}
```
#### Sync files and directories from local to bucket:
```shell
aws s3 sync {{path/to/files}} s3://{{bucket_name}}
```
#### Sync files and directories from bucket to local:
```shell
aws s3 sync s3://{{bucket_name}} {{path/to/target}}
```
#### Sync files and directories with exclusions:
```shell
aws s3 sync {{path/to/files}} s3://{{bucket_name}} --exclude {{path/to/file}} --exclude {{path/to/directory}}/*
```
#### Remove file from bucket:
```shell
aws s3 rm s3://{{bucket}}/{{path/to/file}}
```
#### Preview changes only:
```shell
aws s3 {{any_command}} --dryrun
```
{% endraw %}