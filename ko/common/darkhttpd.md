---
layout: default
title: "darkhttpd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="darkhttpd">
  <a href="/ko/common/darkhttpd.html">darkhttpd</a> <a href="#darkhttpd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Darkhttpd 웹 서버.
> 더 많은 정보: <https://unix4lyfe.org/darkhttpd>.

#### 지정된 문서 경로를 제공하는 서버 시작:
```shell
darkhttpd {{경로/문서}}
```
#### 지정된 포트에서 서버 시작(루트가 아닌 사용자로 시작되는 경우 8080포트가 기본값):
```shell
darkhttpd {{경로/문서}} --port {{포트번호}}
```
#### 지정된 IP 주소에서만 수신 (기본적으로 서버는 모든 인터페이스에서 수신):
```shell
darkhttpd {{경로/문서}} --addr {{ip주소}}
```
{% endraw %}