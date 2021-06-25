---
layout: default
title: "ctest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ctest">
  <a href="/ko/common/ctest.html">ctest</a> <a href="#ctest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CMake 테스트 드라이버 프로그램.
> 더 많은 정보: <https://gitlab.kitware.com/cmake/community/wikis/doc/ctest/Testing-With-CTest>.

#### CMake 프로젝트에 정의된 모든 테스트를 실행하며 , 한번에 4개의 작업을 병렬 실행:
```shell
ctest -j{{4}} --output-on-failure
```
#### 사용 가능한 테스트 목록 표시:
```shell
ctest -N
```
#### 이름을 기준으로 단일 테스트를 실행하거나 정규식을 기준으로 필터링:
```shell
ctest --output-on-failure -R '^{{테스트명}}$'
```
{% endraw %}