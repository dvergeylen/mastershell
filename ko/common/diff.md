---
layout: default
title: "diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diff">
  <a href="/ko/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일들과 디렉토리들을 비교한다.

#### 파일들 비교하기 (`이전_파일명`을 `새_파일명`으로 바꾸는 변경점들 목록):
```shell
diff {{이전_파일명}} {{새_파일명}}
```
#### 공백들을 무시하고, 파일들 비교하기:
```shell
diff -w {{이전_파일명}} {{새_파일명}}
```
#### 차이점들을 나란히 보여주는 파일들 비교하기:
```shell
diff -y {{이전_파일명}} {{새_파일명}}
```
#### 통합된 포맷의 차이점들 표시하며 파일들 비교하기 (`git diff`에서 사용되는 것 같이):
```shell
diff -u {{이전_파일명}} {{새_파일명}}
```
#### 재귀적으로 디렉토리들 비교하기 (다른 파일/디렉토리들의 이름 및 파일에 대한 변경점 출력):
```shell
diff -r {{이전_디렉토리명}} {{새_디렉토리명}}
```
#### 디렉토리들을 비교하고, 서로 다른 파일이름만 표시하기:
```shell
diff -rq {{이전_디렉토리명}} {{새_디렉토리명}}
```
{% endraw %}