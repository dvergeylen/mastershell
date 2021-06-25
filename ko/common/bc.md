---
layout: default
title: "bc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bc">
  <a href="/ko/common/bc.html">bc</a> <a href="#bc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 계산기의 기능을 수행합니다.
> 더 많은 정보: <https://manned.org/bc>.

#### 표준 Math 라이브러리를 사용한 대화형 모드에서 계산기 실행하기:
```shell
bc -l
```
#### 계산 결과 표현법:
```shell
bc <<< "(1 + 2) * 2 ^ 2"
```
#### 계산 및 표현되는 소수 자릿수를 10으로 지정하기:
```shell
bc <<< "scale=10; 5 / 3"
```
#### mathlib를 사용하여 sin 및 cosine의 계산식 표현하기:
```shell
bc -l <<< "s(1) + c(1)"
```
{% endraw %}