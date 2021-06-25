---
layout: default
title: "ar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ar">
  <a href="/ko/common/ar.html">ar</a> <a href="#ar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 아카이브로부터 생성, 수정, 추출 (`.a`, `.so`, `.o`).
> 더 많은 정보: <https://manned.org/ar>.

#### 보관소로부터 모든 멤버를 추출하기:
```shell
ar -x {{libfoo.a}}
```
#### 보관소 멤버 리스트 보여주기:
```shell
ar -t {{libfoo.a}}
```
#### 보관소로 파일을 대체하거나 추가하기:
```shell
ar -r {{libfoo.a}} {{foo.o}} {{bar.o}} {{baz.o}}
```
#### object 파일 인덱스 삽입( `ranlib` 와 같은 기능입니다):
```shell
ar -s {{libfoo.a}}
```
#### 파일 및 첨부된 객체 파일 색인을 사용하여 보관소에 작성:
```shell
ar -rs {{libfoo.a}} {{foo.o}} {{bar.o}} {{baz.o}}
```
{% endraw %}