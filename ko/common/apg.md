---
layout: default
title: "apg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apg">
  <a href="/ko/common/apg.html">apg</a> <a href="#apg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 임의로 복잡한 랜덤 암호를 만듭니다.
> 더 많은 정보: <https://manned.org/apg>.

#### 임의 비밀번호 생성 (기본 비밀번호 길이는 8):
```shell
apg
```
#### 1개 이상의 기호(S), 1개의 숫자(N), 1개의 대문자(C), 1개의 소문자(L) 로 비밀번호 생성:
```shell
apg -M SNCL
```
#### 16개 글자의 비밀번호 생성:
```shell
apg -m {{16}}
```
#### 최대 길이가 16인 비밀번호 생성:
```shell
apg -x {{16}}
```
#### 사전에 나타나지 않는 암호를 생성(사전 파일을 제공해야함):
```shell
apg -r {{디렉토리_파일}}
```
{% endraw %}