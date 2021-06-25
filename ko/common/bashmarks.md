---
layout: default
title: "bashmarks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bashmarks">
  <a href="/ko/common/bashmarks.html">bashmarks</a> <a href="#bashmarks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 하나의 문자 명령을 사용하여 일반적으로 사용되는 디렉토리를 저장하고 점프하십시오.
> 더 많은 정보: <https://github.com/huyng/bashmarks>.

#### 사용 가능한 북마크 나열:
```shell
l
```
#### 현재 디렉토리를 "bookmark_name"으로 저장:
```shell
s {{bookmark_name}}
```
#### 북마크된 디렉토리로 이동:
```shell
g {{bookmark_name}}
```
#### 북마크 된 디렉토리 내용 출력:
```shell
p {{bookmark_name}}
```
#### 북마크 삭제:
```shell
d {{bookmark_name}}
```
{% endraw %}