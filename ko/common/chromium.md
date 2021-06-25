---
layout: default
title: "chromium"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chromium">
  <a href="/ko/common/chromium.html">chromium</a> <a href="#chromium"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 구글에서 제공하는 오픈소스 웹 브라우저.
> 더 많은 정보: <https://chromium.org>.

#### 파일 열기:
```shell
chromium {{경로/파일명.html}}
```
#### URL 열기:
```shell
chromium {{example.com}}
```
#### 익명으로 열기:
```shell
chromium --incognito {{example.com}}
```
#### 새 창에서 열기:
```shell
chromium --new-window {{example.com}}
```
#### 앱 모드로 열기 (툴바, URL 바, 버튼 등 제외):
```shell
chromium --app='{{https://example.com}}'
```
#### 프록시 서버 사용:
```shell
chromium --proxy-server="{{socks5://hostname:66}}" {{example.com}}
```
{% endraw %}