---
layout: default
title: "aws s3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-s3">
  <a href="/ko/common/aws-s3.html">aws s3</a> <a href="#aws-s3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> AWS S3용 CLI - 웹 서비스 인터페이스를 통해 스토리지를 제공합니다.
> 더 많은 정보: <https://aws.amazon.com/cli>.

#### 버킷 안의 파일 보기:
```shell
aws s3 ls {{bucket_name}}
```
#### 로컬에서 버킷으로 파일 및 디렉토리 동기화:
```shell
aws s3 sync {{path/to/files}} s3://{{bucket_name}}
```
#### 버킷에서 로컬로 파일 및 디렉토리 동기화:
```shell
aws s3 sync s3://{{bucket_name}} {{path/to/target}}
```
#### 제외 된 파일 및 디렉토리 동기화:
```shell
aws s3 sync {{path/to/files}} s3://{{bucket_name}} --exclude {{path/to/file}} --exclude {{path/to/directory}}/*
```
#### 버킷에서 파일 제거:
```shell
aws s3 rm s3://{{bucket}}/{{path/to/file}}
```
#### 변경 사항만 미리보기:
```shell
aws s3 {{any_command}} --dryrun
```
{% endraw %}