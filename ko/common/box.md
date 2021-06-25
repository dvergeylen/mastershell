---
layout: default
title: "box"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="box">
  <a href="/ko/common/box.html">box</a> <a href="#box"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Phar의 빌드 및 관리를 위한 PHP 어플리케이션.
> 더 많은 정보: <https://box-project.github.io/box2>.

#### 새 Phar 파일 작성:
```shell
box build
```
#### 특정 구성 파일을 사용하여 새 Phar 파일 작성:
```shell
box build -c {{config/의/경로}}
```
#### PHAR PHP 확장에 대한 정보 표시:
```shell
box info
```
#### 특정 Phar 파일에 대한 정보 표시:
```shell
box info {{phar_파일/의/경로}}
```
#### 현재 작업 디렉토리에서 처음으로 발견된 구성 파일 확인:
```shell
box validate
```
#### 특정 Phar 파일의 서명 확인:
```shell
box verify {{phar_파일/의/경로}}
```
#### 사용 가능한 모든 명령 및 옵션 표시:
```shell
box help
```
{% endraw %}