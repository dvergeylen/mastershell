---
layout: default
title: "bzip2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bzip2">
  <a href="/ko/common/bzip2.html">bzip2</a> <a href="#bzip2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 블록 정렬 파일 압축기.
> 더 많은 정보: <http://bzip.org>.

#### 파일 압축하기:
```shell
bzip2 {{경로/압축할_파일명}}
```
#### 파일 압축해제하기:
```shell
bzip2 -d {{경로/압축된_.bz2파일}}
```
#### 파일을 표준 출력으로 압축해제:
```shell
bzip2 -dc {{경로/압축된_.bz2파일}}
```
{% endraw %}