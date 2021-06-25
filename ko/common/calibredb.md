---
layout: default
title: "calibredb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calibredb">
  <a href="/ko/common/calibredb.html">calibredb</a> <a href="#calibredb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 전자책 데이터베이스를 조작하는 도구.
> Calibre 전자책 라이브러리의 일부.
> 더 많은 정보: <https://manual.calibre-ebook.com/generated/en/calibredb.html>.

#### 도서관의 전자책들을 추가 정보와 함께 리스트로 출력:
```shell
calibredb list
```
#### 추가 정보를 표시하며 전자책 검색:
```shell
calibredb list --search {{검색_용어}}
```
#### 전자책의 ID만 검색:
```shell
calibredb search {{검색_용어}}
```
#### 라이브러리에 전자책 하나 이상 추가하기:
```shell
calibredb add {{파일명1 파일명2 …}}
```
#### 라이브러리에서 전자책을 하나 이상 제거하기. 전자책 ID 필요(위를 참조하시오):
```shell
calibredb remove {{id1 id2 …}}
```
{% endraw %}