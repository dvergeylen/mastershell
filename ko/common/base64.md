---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/ko/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일 또는 표준 입력을 Base64와 표준 출력으로 인코딩하거나 디코딩함.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/base64>.

#### 파일 인코딩:
```shell
base64 {{filename}}
```
#### 파일 디코딩:
```shell
base64 --decode {{filename}}
```
#### stdin에서 인코딩:
```shell
{{somecommand}} | base64
```
#### stdin에서 디코딩:
```shell
{{somecommand}} | base64 --decode
```
{% endraw %}