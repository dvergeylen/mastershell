---
layout: default
title: "abduco"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="abduco">
  <a href="/ko/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 터미널 세션 관리자.
> 더 많은 정보: <http://www.brain-dump.org/projects/abduco/>.

#### 세션 목록:
```shell
abduco
```
#### 세션에 연결하기, 만약 존재하지 않는 경우에는 생성:
```shell
abduco -A {{name}} {{bash}}
```
#### `dvtm`으로 세션 연결하기, 만약 존재하지 않는 경우에는 생성:
```shell
abduco -A {{name}}
```
#### 세션으로부터 제거:
```shell
Ctrl + \
```
#### 읽기 전용 모드로 세션 연결하기:
```shell
abduco -Ar {{name}}
```
{% endraw %}