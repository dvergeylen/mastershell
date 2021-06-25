---
layout: default
title: "act"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="act">
  <a href="/ko/common/act.html">act</a> <a href="#act"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker를 사용하여 로컬로 GitHub작업 실행.
> 더 많은 정보: <https://github.com/nektos/act>.

#### 가능한 작업들 목록:
```shell
act -l
```
#### 기본 이벤트 실행:
```shell
act
```
#### 특정 이벤트 실행:
```shell
act {{event_type}}
```
#### 특정 작업 실행:
```shell
act -a {{action_id}}
```
#### 실제론 작업을 실행하지 않기 (예 : a dry run):
```shell
act -n
```
#### 자세한 로그 표시:
```shell
act -v
```
{% endraw %}