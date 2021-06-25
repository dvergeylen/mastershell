---
layout: default
title: "cloc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cloc">
  <a href="/ko/common/cloc.html">cloc</a> <a href="#cloc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 소스코드와 주석의 줄 개수를 세고 차이를 계산합니다.
> 더 많은 정보: <https://github.com/AlDanial/cloc>.

#### 디렉토리 안의 모든 코드의 줄 개수를 셉니다:
```shell
cloc {{/경로/디렉토리}}
```
#### 진행 바로 현재 진행 중인 과정을 보여주면서 디렉토리 안의 모든 코드의 줄 개수를 셉니다:
```shell
cloc --progress=1 {{/경로/디렉토리}}
```
#### 두 개의 디렉토리 구조를 비교하고 차이의 개수를 셉니다:
```shell
cloc --diff {{/디렉토리/첫번째}} {{/디렉토리/두번째}}
```
{% endraw %}