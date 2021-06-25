---
layout: default
title: "csvstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvstat">
  <a href="/ko/common/csvstat.html">csvstat</a> <a href="#csvstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> csvkit에 포함된 CSV 파일의 모든 열에 대한 설명 통계 출력.
> 더 많은 정보: <https://csvkit.readthedocs.io/en/latest/scripts/csvstat.html>.

#### 모든 열에 대한 정보 출력:
```shell
csvstat {{데이터.csv}}
```
#### 2열 , 4열의 모든 정보 출력:
```shell
csvstat -c {{2,4}} {{데이터.csv}}
```
#### 모든 열의 합계 출력:
```shell
csvstat --sum {{data.csv}}
```
#### 3열에 대한 최대값 길이 출력:
```shell
csvstat -c {{3}} --len {{데이터.csv}}
```
#### "이름" 열에 고유 값의 수 출력:
```shell
csvstat -c {{이름}} --unique {{데이터.csv}}
```
{% endraw %}