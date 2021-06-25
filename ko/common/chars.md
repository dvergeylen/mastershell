---
layout: default
title: "chars"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chars">
  <a href="/ko/common/chars.html">chars</a> <a href="#chars"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 다양한 ASCII 및 유니코드 문자 및 코드 포인트에 대한 이름 및 코드 표시.
> 더 많은 정보: <https://github.com/antifuchs/chars>.

#### 밸류 값으로 문자 검색:
```shell
chars '{{ß}}'
```
#### 유니코드 코드로 문자 검색:
```shell
chars {{U+1F63C}}
```
#### 모호한 코드 포인트가 주어지면 가능한 문자 검색:
```shell
chars {{10}}
```
#### 제어 문자 찾기:
```shell
chars "{{^C}}"
```
{% endraw %}