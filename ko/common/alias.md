---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/ko/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 명령 문자열로 대체되는 단어인 별칭 -- 작성.
> 별칭은 셀의 구성 파일에 정의되어 있지 않으면 현재 쉘 세션으로 만료됩니다, 예 : `~/.bashrc`.
> 더 많은 정보: <https://tldp.org/LDP/abs/html/aliases.html>.

#### 모든 별칭 리스트:
```shell
alias
```
#### 일반 별칭 생성:
```shell
alias {{단어}}="{{명령어}}"
```
#### 주어진 별칭에 연관된 명령어:
```shell
alias {{단어}}
```
#### 별칭 명령어 제거:
```shell
unalias {{단어}}
```
#### `rm` 을 대화형 명령어로 전환:
```shell
alias {{rm}}="{{rm -i}}"
```
#### `ls -a`의 지름길인 `la`생성:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}