---
layout: default
title: "cowsay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cowsay">
  <a href="/ko/common/cowsay.html">cowsay</a> <a href="#cowsay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 무언가를 말하거나 생각하는 ASCII 문자(기본적으로 cow)를 생성.
> 더 많은 정보: <https://github.com/tnalpgge/rank-amateur-cowsay>.

#### "Hello world"라고 말하는 ASCII cow 출력:
```shell
cowsay "Hello world"
```
#### 풍선에 표준 입력의 텍스트 사용:
```shell
echo "Hello" | cowsay
```
#### 사용 가능한 모든 문자 나열:
```shell
cowsay -l
```
#### "Hello"라고 말하는 ASCII dragon 출력:
```shell
cowsay -f dragon "Hello"
```
#### 돌로 된 생각하는 ASCII cow 출력:
```shell
cowthink -s "I'm just a cow, not a great thinker..."
```
{% endraw %}