---
layout: default
title: "csvsort"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvsort">
  <a href="/ko/common/csvsort.html">csvsort</a> <a href="#csvsort"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> csvkit에 포함된 CSV 파일을 정렬.
> 더 많은 정보: <https://csvkit.readthedocs.io/en/latest/scripts/csvsort.html>.

#### CSV 파일을 9열을 기준으로 정렬:
```shell
csvsort -c {{9}} {{데이터.csv}}
```
#### CSV 파일을 "이름" 열에 따라 내림차순으로 정렬:
```shell
csvsort -r -c {{이름}} {{데이터.csv}}
```
#### CSV 파일을 2열, 4열을 기준으로 정렬:
```shell
csvsort -c {{2,4}} {{데이터.csv}}
```
#### 데이터 형식과 관계 없이 CSV 파일 정렬:
```shell
csvsort --no-inference -c {{열}} {{데이터.csv}}
```
{% endraw %}