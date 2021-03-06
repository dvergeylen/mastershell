---
layout: default
title: "cut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cut">
  <a href="/ko/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> stdin 혹은 파일에서 출력 필드를 자른다.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/cut>.

#### stdin의 각 라인에 첫번째 16개의 문자를 자르기:
```shell
cut -c {{1-16}}
```
#### 지정된 파일의 각 라인의 첫번째 16개 문자를 자르기:
```shell
cut -c {{1-16}} {{파일}}
```
#### 3번째 문자 부터 각 라인의 끝까지 모든 문자를 자르기:
```shell
cut -c {{3-}}
```
#### `:` 을 필드 구분 기호로 사용하여 각 라인의 5번째 필드를 자르기(기본 구분 기호 : 탭):
```shell
cut -d'{{:}}' -f{{5}}
```
#### `;` 을 구분 기호로 사용하여 각 라인의 2번째와 10번째 필드를 자르기:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### 공백을 구분 기호로 사용하여 각 라인의 끝까지 필드 3을 자르기:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}