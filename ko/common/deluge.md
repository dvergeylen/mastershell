---
layout: default
title: "deluge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluge">
  <a href="/ko/common/deluge.html">deluge</a> <a href="#deluge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> BitTorrent 클라이언트 명령어.
> 더 많은 정보: <https://deluge-torrent.org/>.

#### 토렌트 다운로드:
```shell
deluge {{url|마그넷|경로/파일명}}
```
#### 특정 구성 파일을 사용하여 토렌트를 다운로드하십시오:
```shell
deluge -c {{경로/구성_파일}} {{url|마그넷|경로/파일명}}
```
#### 토렌트를 다운로드하고 지정된 사용자 인터페이스로 시작:
```shell
deluge -u {{gtk|웹|콘솔}} {{url|마그넷|경로/파일명}}
```
#### 토렌트를 다운로드하고 로그를 파일로 출력:
```shell
deluge -l {{경로/로그_파일}} {{url|마그넷|경로/파일명}}
```
{% endraw %}