---
layout: default
title: "date"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="date">
  <a href="/ko/common/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 시스템 날짜 설정 및 표시.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/date>.

#### 기본 로컬 형식을 사용하여 현재 날짜 표시:
```shell
date +"%c"
```
#### 현재 날짜를 UTC 및 ISO 8601 형식으로 표시:
```shell
date -u +"%Y-%m-%dT%H:%M:%SZ"
```
#### 현재 날짜를 Unix 타임스탬프로 표시 (Unix epoch 이후 몇 초):
```shell
date +%s
```
#### 기본 형식을 사용하여 특정 날짜 표시(Unix 타임스탬프로 표시):
```shell
date -d @1473305798
```
#### 특정 날짜를 Unix 타임스탬프 형식으로 변환:
```shell
date -d "{{2018-09-01 00:00}}" +%s --utc
```
{% endraw %}