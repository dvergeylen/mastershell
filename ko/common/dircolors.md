---
layout: default
title: "dircolors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dircolors">
  <a href="/ko/common/dircolors.html">dircolors</a> <a href="#dircolors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> LS_COLOR 환경변수와 스타일 `ls`, `dir`, 등을 설정하기 위한 명령어들을 출력한다.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/dircolors>.

#### 기본 색상을 사용하여 LS_COLOR를 설정하는 명령어들 출력하기:
```shell
dircolors
```
#### 파일로부터 색상을 사용하여 LS_COLOR를 설정하는 명령어들 출력하기:
```shell
dircolors {{파일명}}
```
#### Bourne 쉘에 관한 명령어들 출력:
```shell
dircolors --bourne-shell
```
#### C 쉘에 관한 명령어들 출력:
```shell
dircolors --c-shell
```
#### 파일 유형과 확장에 대한 기본 색상들 보기:
```shell
dircolors --print-data
```
{% endraw %}