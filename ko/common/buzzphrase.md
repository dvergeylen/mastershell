---
layout: default
title: "buzzphrase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="buzzphrase">
  <a href="/ko/common/buzzphrase.html">buzzphrase</a> <a href="#buzzphrase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 임의의 buzzphrase를 출력하는 Node.js 명령 줄 도구.
> 더 많은 정보: <https://github.com/atomantic/buzzphrase>.

#### 형용사, 과거시제 동사 및 복수 명사를 포함하는 세 개의 임의 구문으로 이루어진 문자열 생성:
```shell
buzzphrase
```
#### 동사의 명령형[i] + 동사의 과거시제[v] + 형용사[a] + 복수형 명사[N] 형태로 포맷된 구문 출력:
```shell
buzzphrase {{'{i} {v} {a} {N}'}}
```
#### 현재분사 동사[V] + 형용사[a] + 단수형 명사[n] + 마침[f] 형태로 포맷된 4개의 구문 출력:
```shell
buzzphrase {{4 '{V} {a} {n} {f}'}}
```
{% endraw %}