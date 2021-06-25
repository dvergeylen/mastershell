---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/ko/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일 출력 및 연결.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/cat>.

#### 표준출력으로 파일 내용 출력:
```shell
cat {{파일명}}
```
#### 여러 파일을 대상 파일에 연결:
```shell
cat {{파일명1}} {{파일명2}} > {{대상_파일명}}
```
#### 대상 파일에 여러 파일 내용 추가:
```shell
cat {{파일명1}} {{파일명2}} >> {{대상_파일명}}
```
#### 모든 출력 라인에 번호 매기기:
```shell
cat -n {{파일명}}
```
#### 출력할 수 없는 문자 및 공백 문자 표시 (ASCII가 아닌 경우 `M-`접두사 포함):
```shell
cat -v -t -e {{파일명}}
```
{% endraw %}