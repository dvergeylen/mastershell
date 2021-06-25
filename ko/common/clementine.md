---
layout: default
title: "clementine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clementine">
  <a href="/ko/common/clementine.html">clementine</a> <a href="#clementine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 현대적인 음악 플레이어이자 라이브러리 생성자.
> 더 많은 정보: <https://www.clementine-player.org>.

#### Clementine 열기:
```shell
clementine
```
#### 음악 파일을 실행합니다:
```shell
clementine {{url_혹은_경로/파일.ext}}
```
#### 정지, 재생 버튼(Toggle):
```shell
clementine --play-pause
```
#### 재생 멈추기:
```shell
clementine --stop
```
#### 다음 트랙 넘기기:
```shell
clementine --next
```
#### 이전 트랙 넘기기:
```shell
clementine --previous
```
#### 플레이리스트 파일 불러오기:
```shell
clementine --load {{경로/재생리스트.ext}}
```
#### 현재 불러온 플레이리스트에서 5번째 트랙 재생하기:
```shell
clementine --play-track {{5}}
```
{% endraw %}