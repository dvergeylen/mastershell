---
layout: default
title: "airpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airpaste">
  <a href="/ko/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 동일 네트워크 내에서 메시지와 파일들 공유.
> 더 많은 정보: <https://github.com/mafintosh/airpaste>.

#### 메시지 대기와 수신 시 표시:
```shell
airpaste
```
#### 텍스트 보내기:
```shell
echo {{텍스트}} | airpaste
```
#### 파일 보내기:
```shell
airpaste < {{경로/파일명}}
```
#### 파일 내려받기:
```shell
airpaste > {{경로/파일명}}
```
#### 채널 만들기/접속하기:
```shell
airpaste {{채널_이름}}
```
{% endraw %}