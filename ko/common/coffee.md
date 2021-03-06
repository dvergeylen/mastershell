---
layout: default
title: "coffee"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="coffee">
  <a href="/ko/common/coffee.html">coffee</a> <a href="#coffee"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Coffee Script를 실행하거나 JavaScript로 컴파일합니다.
> 더 많은 정보: <https://coffeescript.org#cli>.

#### 스크립트 실행:
```shell
coffee {{경로/파일.coffee}}
```
#### JavaScript로 컴파일 하거나 같은 이름의 파일로 저장합니다:
```shell
coffee --compile {{경로/파일.coffee}}
```
#### JavaScript로 컴파일 하거나 주어진 출력 파일로 저장합니다:
```shell
coffee --compile {{경로/파일.coffee}} --output {{경로/파일.js}}
```
#### 대화형 REPL 실행:
```shell
coffee --interactive
```
#### 스크립트의 변화를 보거나 다시 실행합니다:
```shell
coffee --watch {{경로/파일.coffee}}
```
{% endraw %}