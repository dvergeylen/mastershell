---
layout: default
title: "black"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="black">
  <a href="/ko/common/black.html">black</a> <a href="#black"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python 자동 코드 formatter.
> 더 많은 정보: <https://github.com/psf/black>.

#### 파일 또는 전체 디렉토리의 자동 포맷:
```shell
black {{파일_또는_디렉토리/의/경로}}
```
#### 전달된 코드를 문자열로 포맷:
```shell
black -c {{파일_또는_디렉토리/의/경로}}
```
#### 표준 출력시 각 파일에 대해 diff 출력:
```shell
black --diff {{파일_또는_디렉토리/의/경로}}
```
#### 파일을 다시 쓰지 않고 상태 반환:
```shell
black --check {{파일_또는_디렉토리/의/경로}}
```
#### 파일 또는 디렉토리가 stderr에 배타적 오류 메시지를 발생시키는 자동 포맷:
```shell
black --quiet {{파일_또는_디렉토리/의/경로}}
```
{% endraw %}