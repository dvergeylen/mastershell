---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/ko/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 높은 파일압축률을 보여주는 압축 프로그램.
> .7z파일들만을 지원하는 `7z`의 독립형 버전.
> 더 많은 정보: <https://www.7-zip.org/>.

#### 파일이나 디렉토리 압축하기:
```shell
7zr a {{archived.7z}} {{경로/파일명_또는_디렉토리명}}
```
#### 기존 디렉토리 경로에 존재하는 7z파일 추출하기:
```shell
7zr x {{archived.7z}}
```
#### 압축 파일의 내용 리스트:
```shell
7zr l {{archived.7z}}
```
{% endraw %}