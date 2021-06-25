---
layout: default
title: "copyq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="copyq">
  <a href="/ko/common/copyq.html">copyq</a> <a href="#copyq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 고급 기능을 갖춘 클립보드 매니저.
> 더 많은 정보: <https://hluk.github.io/CopyQ/>.

#### copyQ를 시작하여 클립보드 기록 저장:
```shell
copyq
```
#### 현재 클립보드 내용 표시:
```shell
copyq clipboard
```
#### 클립보드 기록에 원본 텍스트 삽입:
```shell
copyq add -- {{텍스트1}} {{텍스트2}} {{텍스트3}}
```
#### 이스케이프 시퀀스 ('\n', '\t')가 포함 된 텍스트를 클립보드 기록에 삽입:
```shell
copyq add {{첫째 줄\n둘째 줄}}
```
#### 클립보드 기록에서 처음 3개 항목의 내용을 출력:
```shell
copyq read 0 1 2
```
#### 파일 내용을 클립보드에 복사:
```shell
copyq copy < {{파일.txt}}
```
#### JPEG 이미지를 클립보드에 복사:
```shell
copyq copy image/jpeg < {{이미지.jpg}}
```
{% endraw %}