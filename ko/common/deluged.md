---
layout: default
title: "deluged"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluged">
  <a href="/ko/common/deluged.html">deluged</a> <a href="#deluged"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deluge BitTorrent 클라이언트를 위한 데몬 프로세스.
> 더 많은 정보: <https://deluge-torrent.org/>.

#### Deluge 데몬 시작하기:
```shell
deluged
```
#### 특정 포트에서 Deluge 데몬 시작하기:
```shell
deluged -p {{포트번호}}
```
#### 특정 구성파일을 이용하여 Deluge 데몬 시작하기:
```shell
deluged -c {{경로/구성_파일명}}
```
#### Deluge 데몬을 시작하고 파일에 로그 출력하기:
```shell
deluged -l {{경로/로그_파일명}}
```
{% endraw %}