---
layout: default
title: "complete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="complete">
  <a href="/ko/common/complete.html">complete</a> <a href="#complete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 쉘 명령어에 자동 완성 인자를 제공합니다.
> 더 많은 정보: <https://www.gnu.org/software/bash/manual/html_node/Programmable-Completion-Builtins.html>.

#### 함수에 명령어 자동 완성 기능을 적용합니다:
```shell
complete -F {{함수}} {{명령어}}
```
#### 다른 명령어에 명령어 자동 완성 기능을 적용합니다:
```shell
complete -C {{자동완성_명령어}} {{명령어}}
```
#### 작성 완료된 단어에 공백을 추가하지 않고 자동 완성 기능을 적용합니다:
```shell
complete -o nospace -F {{함수}} {{명령어}}
```
{% endraw %}