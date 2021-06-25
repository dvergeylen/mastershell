---
layout: default
title: "deluser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluser">
  <a href="/ko/linux/deluser.html">deluser</a> <a href="#deluser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 유저 계정 제거 또는 그룹으로부터 사용자 제거.
> 더 많은 정보: <https://manpages.debian.org/latest/adduser/deluser.html>.

#### 유저 삭제:
```shell
deluser {{이름}}
```
#### 사용자의 홈 디렉토리 및 메일 스풀과 함께 사용자 제거:
```shell
deluser -r {{이름}}
```
#### 그룹으로부터 사용자 제거:
```shell
deluser {{이름}} {{그룹}}
```
{% endraw %}