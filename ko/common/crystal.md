---
layout: default
title: "crystal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="crystal">
  <a href="/ko/common/crystal.html">crystal</a> <a href="#crystal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crystal 소스 코드를 위한 관리도구.
> 더 많은 정보: <https://crystal-lang.org/reference/using_the_compiler>.

#### Crystal 파일 실행:
```shell
crystal {{경로/파일.cr}}
```
#### 단일 실행 파일로의 종속성 및 파일 컴파일:
```shell
crystal build {{경로/파일.cr}}
```
#### 언어 테스트를 위한 로컬 대화형 서버 시작:
```shell
crystal play
```
#### Cystal 응용 프로그램을 위한 프로젝트 디렉토리 생성:
```shell
crystal init app {{어플리케이션명}}
```
#### 도움말 옵션 표시:
```shell
crystal help
```
{% endraw %}