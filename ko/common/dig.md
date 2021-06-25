---
layout: default
title: "dig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dig">
  <a href="/ko/common/dig.html">dig</a> <a href="#dig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DNS 조회 유틸리티.
> 더 많은 정보: <https://manpages.debian.org/dnsutils/dig.1.html>.

#### 호스트이름과 관련된 IP 조회하기 (A records):
```shell
dig +short {{example.com}}
```
#### 주어진 도메인 이름과 관련된 메일 서버 조회하기 (MX record):
```shell
dig +short {{example.com}} MX
```
#### 주어진 도메인 이름에 대한 모든 유형의 레코드들 가져오기:
```shell
dig {{example.com}} ANY
```
#### 쿼리할 대체 DNS 서버를 지정하기:
```shell
dig @{{8.8.8.8}} {{example.com}}
```
#### IP 주소에서 역방향 DNS 조회하기 (PTR record):
```shell
dig -x {{8.8.8.8}}
```
#### 영역에 대해 권한있는 이름 서버들을 찾고 SOA 레코드들 표시하기:
```shell
dig +nssearch {{example.com}}
```
#### 반복적인 쿼리들을 수행하고 도메인 이름을 분석하기 위해 전체 추적 경로를 표시하기:
```shell
dig +trace {{example.com}}
```
{% endraw %}