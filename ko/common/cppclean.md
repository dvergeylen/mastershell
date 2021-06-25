---
layout: default
title: "cppclean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cppclean">
  <a href="/ko/common/cppclean.html">cppclean</a> <a href="#cppclean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> C++ 프로젝트에서 사용하지 않는 코드 찾기.
> 더 많은 정보: <https://github.com/myint/cppclean>.

#### 프로젝트 디렉토리에서 실행:
```shell
cppclean {{프로젝트/의/경로}}
```
#### 헤더가 `inc1/` 및 `inc2/` 디렉토리에 있는 프로젝트에서 실행:
```shell
cppclean {{프로젝트/의/경로}} --include-path={{inc1}} --include-path={{inc2}}
```
#### 특정 팡리 `main.cpp`에서 실행:
```shell
cppclean {{main.cpp}}
```
#### `build`디렉토리를 제외한 현재 디렉토리에서 실행:
```shell
cppclean {{.}} --exclude={{build}}
```
{% endraw %}