---
layout: default
title: "bg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bg">
  <a href="/ko/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 일시 중단된 작업을 다시 시작하고 (예. `Ctrl + Z`), 그 작업이 background에서 동작하게 유지.
> 더 많은 정보: <https://manned.org/bg>.

#### 가장 최근에 일시 중단된 작업을 재개하고 background에서 실행:
```shell
bg
```
#### 특정 작업을 재개하고(`jobs -l` 를 사용하여 ID 가져오기) background에서 실행:
```shell
bg %{{job_id}}
```
{% endraw %}