---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/ko/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 프로그래머에게 최적화된 grep과 같은 검색툴.
> 더 많은 정보: <https://beyondgrep.com/documentation/>.

#### "foo"를 포함하고 있는 파일 검색:
```shell
ack {{foo}}
```
#### 특정 타입의 파일 검색:
```shell
ack --ruby {{foo}}
```
#### "foo"라는 용어와 일치하는 총 합을 계산:
```shell
ack -ch {{foo}}
```
#### "foo"를 포함하고있는 파일의 이름과 각각 파일에서 일치하는 수를 표시:
```shell
ack -cl {{foo}}
```
#### 모든 가능한 타입 리스트:
```shell
ack --help-types
```
{% endraw %}