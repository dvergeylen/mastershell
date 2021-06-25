---
layout: default
title: "detox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="detox">
  <a href="/ko/common/detox.html">detox</a> <a href="#detox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 작업하기 쉽도록 파일 이름을 다시 설정합니다.
> 그것은 공백과 다른 중복된 밑줄 문자같은 골칫거리들을 제거한다.
> 더 많은 정보: <https://github.com/dharple/detox>.

#### 파일의 이름으로부터 공백과 다른 바람직하지 않은 문자들을 제거:
```shell
detox {{파일명}}
```
#### detox가 디렉토리 트리에서 모든 파일 이름을 재설정하는 방법 출력:
```shell
detox --dry-run -r {{디렉토리명}}
```
#### 디렉토리 트리에서 모든 파일들로부터 공백과 다른 바람직하지 않은 문자들을 제거:
```shell
detox -r {{디렉토리명}}
```
{% endraw %}