---
layout: default
title: "dep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dep">
  <a href="/ko/common/dep.html">dep</a> <a href="#dep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Go 프로젝트에서 종속성 관리를 위한 툴.
> 더 많은 정보: <https://golang.github.io/dep>.

#### 현재 디렉토리를 Go 프로젝트의 루트 디렉토리로 초기화:
```shell
dep init
```
#### 누락된 종속성 설치(Gopkg.toml 과 .go 파일들 스캔):
```shell
dep ensure
```
#### 프로젝트의 종속성의 상태 보고:
```shell
dep status
```
#### 프로젝트에 종속성 추가:
```shell
dep ensure -add {{패키지_url}}
```
#### 모든 종속성들의 잠긴 버전 업데이트:
```shell
dep ensure -update
```
{% endraw %}