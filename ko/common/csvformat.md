---
layout: default
title: "csvformat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvformat">
  <a href="/ko/common/csvformat.html">csvformat</a> <a href="#csvformat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> csvkit에 포함된 CSV 파일을 사용자 정의 출력으로 변환.
> 더 많은 정보: <https://csvkit.readthedocs.io/en/latest/scripts/csvformat.html>.

#### 탭으로 구분된 파일(TSV)로 변환:
```shell
csvformat -T {{데이터.csv}}
```
#### 구분자를 사용자 지정 문자로 변환:
```shell
csvformat -D "{{사용자_지정_문자}}" {{데이터.csv}}
```
#### 라인의 끝을 캐리지 리턴 (^M) + 라인 바꿈으로 변환:
```shell
csvformat -M "{{\r\n}}" {{데이터.csv}}
```
#### 인용문 사용 최소화:
```shell
csvformat -U 0 {{데이터.csv}}
```
#### 인용문 사용 최대화:
```shell
csvformat -U 1 {{데이터.csv}}
```
{% endraw %}