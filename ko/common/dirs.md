---
layout: default
title: "dirs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirs">
  <a href="/ko/common/dirs.html">dirs</a> <a href="#dirs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 디렉토리 스택을 표시하거나 조작한다.
> 디렉토리 스택은 `pushd`과 `popd` 명령어로 조작할 수 있는 최근 방문한 디렉토리의 목록이다.
> 더 많은 정보: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

#### 각각의 엔트리 사이에서 공백으로 디렉토리 스택을 표시하기:
```shell
dirs
```
#### 하나의 엔트리에 하나의 라인으로 디렉토리 스택 표시하기:
```shell
dirs -p
```
#### 0부터 시작하는 디렉토리 스택에 n번째 항만 표시하기:
```shell
dirs +{{N}}
```
#### 디렉토리 스택 초기화하기:
```shell
dirs -c
```
{% endraw %}