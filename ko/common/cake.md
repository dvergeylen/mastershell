---
layout: default
title: "cake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cake">
  <a href="/ko/common/cake.html">cake</a> <a href="#cake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CakePHP 프레임 워크용 명령어 라인 프로세서.
> 더 많은 정보: <https://cakephp.org>.

#### 현재 앱 및 사용 가능한 명령어에 대한 기본 정보 표시:
```shell
cake
```
#### 사용 가능한 경로 리스트 표시:
```shell
cake routes
```
#### 구성 캐시 지우기:
```shell
cake cache clear_all
```
#### 메타데이터 캐시 구축:
```shell
cake schema_cache build --connection {{연결할것}}
```
#### 메타데이터 캐시 지우기:
```shell
cake schema_cache clear
```
#### 단일 캐시 테이블 지우기:
```shell
cake schema_cache clear {{테이블_이름}}
```
#### 개발 웹 서버 시작 (포트 기본값 8765):
```shell
cake server
```
#### REPL 대화형 쉘 인스턴스 시작:
```shell
cake console
```
{% endraw %}