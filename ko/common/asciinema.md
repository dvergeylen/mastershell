---
layout: default
title: "asciinema"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciinema">
  <a href="/ko/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 터미널 세션을 녹음하고 재생하며 선택적으로 asciinema.org에서 공유합니다.
> 더 많은 정보: <https://asciinema.org/>.

#### `asciinema` 로컬 설치와 with an asciinema.org 계정을 연결하기:
```shell
asciinema auth
```
#### 새로운 녹음을 작성 (한 번 완료되면 사용자는 업로드하거나 로컬로 저장하라는 메시지가 표시됩니다):
```shell
asciinema rec
```
#### 새 녹음을 만들고 로컬 파일에 저장:
```shell
asciinema rec {{경로/파일명}}.cast
```
#### 로컬 파일에서 녹음한 터미널을 재생:
```shell
asciinema play {{경로/파일명}}.cast
```
#### asciinema.org에서 호스트된 터미널 녹음을 재생:
```shell
asciinema play https://asciinema.org/a/{{cast_id}}
```
#### 새로운 녹음을 만들어 유휴 시간을 최대 2.5초로 제한:
```shell
asciinema rec -i {{2.5}}
```
#### 로컬 저장 기록의 전체 출력을 인쇄:
```shell
asciinema cat {{경로/파일명}}.cast
```
#### 로컬로 저장된 터미널 세션을 asciinema.org에 업로드하기:
```shell
asciinema upload {{경로/파일명}}.cast
```
{% endraw %}