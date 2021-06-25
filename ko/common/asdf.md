---
layout: default
title: "asdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asdf">
  <a href="/ko/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 여러 패키지 버전을 관리하기 위한 CLI(Command-line Interface) 입니다.
> 더 많은 정보: <https://asdf-vm.com>.

#### 사용 가능한 모든 플러그인을 나열:
```shell
asdf plugin-list-all
```
#### 플러그인 설치:
```shell
asdf plugin-add {{이름}}
```
#### 모든 사용 가능한 패키지 버전 나열:
```shell
asdf list-all {{이름}}
```
#### 특정 패키지 버전 설치:
```shell
asdf install {{이름}} {{버전}}
```
#### 글로벌 버전 패키지 설치:
```shell
asdf global {{버전}} {{버전}}
```
#### 로컬 버전 패키지 설치:
```shell
asdf local {{이름}} {{버전}}
```
{% endraw %}