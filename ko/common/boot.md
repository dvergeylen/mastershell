---
layout: default
title: "boot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="boot">
  <a href="/ko/common/boot.html">boot</a> <a href="#boot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clojure 프로그래밍 언어를 위한 빌드.
> 더 많은 정보: <https://github.com/boot-clj/boot>.

#### 프로젝트 혹은 독립으로 REPL 세션 시작:
```shell
boot repl
```
#### 단일 "uberjar" 구축:
```shell
boot jar
```
#### 명령어 안내:
```shell
boot cljs --help
```
#### 템플릿을 기반으로 새로운 프로젝트에 대한 기반 생성:
```shell
boot --dependencies boot/new new --template {{템플릿명}} --name {{프로젝트명}}
```
#### 개발용 빌드 (부트/새 템플릿을 사용하는 경우):
```shell
boot dev
```
#### 생산용 빌드 (부트/새 템플릿을 사용하는 경우):
```shell
boot prod
```
{% endraw %}