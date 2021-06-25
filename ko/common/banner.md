---
layout: default
title: "banner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="banner">
  <a href="/ko/common/banner.html">banner</a> <a href="#banner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 주어진 인자를 큰 ASCII art로 출력.
> 더 많은 정보: <https://man.archlinux.org/man/banner.1>.

#### 텍스트 메시지를 큰 배너로 출력(따옴표는 선택 사항):
```shell
banner "{{Hello World}}"
```
#### 텍스트 메시지를 너비가 50자인 배너로 출력:
```shell
banner -w {{50}} "{{Hello World}}"
```
#### stdin에서 텍스트 읽기:
```shell
banner
```
{% endraw %}