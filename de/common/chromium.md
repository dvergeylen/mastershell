---
layout: default
title: "chromium"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chromium">
  <a href="/de/common/chromium.html">chromium</a> <a href="#chromium"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open-Source-Webbrowser von Google.
> Weitere Informationen: <https://chromium.org>.

#### Öffne eine html-Datei:
```shell
chromium {{pfad/zu/datei.html}}
```
#### Öffne eine bestimmte URL:
```shell
chromium {{beispiel.com}}
```
#### Öffne eine URL im Inkognito-Modus:
```shell
chromium --incognito {{beispiel.com}}
```
#### Öffne eine URL in einem neuen Fenster:
```shell
chromium --new-window {{beispiel.com}}
```
#### Öffne eine URL im Anwendungsmodus (ohne Symbolleisten, Suchleiste, Schaltflächen usw.):
```shell
chromium --app='{{https://beispiel.com}}'
```
#### Öffne eine URL und verwende einen Proxy-Server:
```shell
chromium --proxy-server="{{socks5://hostname:66}}" {{beispiel.com}}
```
{% endraw %}