---
layout: default
title: "asar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asar">
  <a href="/ko/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 전자 플랫폼을 위한 파일 저장소입니다.
> 더 많은 정보: <https://github.com/electron/asar>.

#### 파일 또는 디렉토리 보관:
```shell
asar pack {{path/to/file_or_directory}} {{archived.asar}}
```
#### 보관소 추출:
```shell
asar extract {{archived.asar}}
```
#### 보관소에서 특정 파일 추출:
```shell
asar extract-file {{archived.asar}} {{file}}
```
#### 보관소 파일의 내용을 나열 :
```shell
asar list {{archived.asar}}
```
{% endraw %}