---
layout: default
title: "cradle package"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-package">
  <a href="/ko/common/cradle-package.html">cradle package</a> <a href="#cradle-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cradle 인스턴스의 패키지 관리.
> 더 많은 정보: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#package>.

#### 사용가능한 패키지 목록 표시:
```shell
cradle package list
```
#### 패키지 검색:
```shell
cradle package search {{패키지}}
```
#### Packagist에서 패키지 설치:
```shell
cradle package install {{패키지}}
```
#### 특정 버전의 패키지 설치:
```shell
cradle package install {{패키지}} {{버전}}
```
#### 패키지 업데이트:
```shell
cradle package update {{패키지}}
```
#### 패키지를 특정 버전으로 업데이트:
```shell
cradle package update {{패키지}} {{버전}}
```
#### 특정 패키지 제거:
```shell
cradle package remove {{패키지}}
```
{% endraw %}