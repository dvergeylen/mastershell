---
layout: default
title: "apropos"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apropos">
  <a href="/ko/common/apropos.html">apropos</a> <a href="#apropos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 메뉴얼 페이지에서 검색, 예를 들어 새로운 명령어 검색.
> 더 많은 정보: <https://manned.org/apropos>.

#### 키워드 검색:
```shell
apropos {{정규 표현식}}
```
#### 출력을 터미널 너비에 제한을 두지 않고 검색:
```shell
apropos -l {{정규 표현식}}
```
#### 주어진 모든 표현식만 포함하는 페이지 검색(AND 검색):
```shell
apropos {{정규 표현식_1}} -a {{정규 표현식_2}} -a {{정규 표현식_3}}
```
{% endraw %}