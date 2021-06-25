---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/ko/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 높은 파일 압축률을 보여주는 파일 압축 프로그램.
> 더 적은 압축 타입을 지원하는 `7z`의 독립형 버전.
> 더 많은 정보: <https://www.7-zip.org/>.

#### 파일이나 디렉토리 압축하기:
```shell
7za a {{archived.7z}} {{path/to/file_or_directory}}
```
#### 기존 디렉토리 경로에 존재하는 7z 파일 추출:
```shell
7za x {{archived}}
```
#### 특정 압축 타입을 이용하여 추출하기:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{archived}} {{path/to/file_or_directory}}
```
#### 사용가능한 압축 타입 리스트:
```shell
7za i
```
#### 압축 파일의 내용 리스트:
```shell
7za l {{archived}}
```
{% endraw %}