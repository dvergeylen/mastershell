---
layout: default
title: "chromium"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chromium">
  <a href="/it/common/chromium.html">chromium</a> <a href="#chromium"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Browser web open-source di Google.
> Maggiori informazioni: <https://chromium.org>.

#### Apri un file:
```shell
chromium {{percorso/al/file.html}}
```
#### Apri un URL:
```shell
chromium {{esempio.com}}
```
#### Apri in modalità incognito:
```shell
chromium --incognito {{esempio.com}}
```
#### Apri in una nuova finestra:
```shell
chromium --new-window {{esempio.com}}
```
#### Apri in modalità app (senza barre degli strumenti, URL, bottoni, etc.):
```shell
chromium --app='{{https://esempio.com}}'
```
#### Usa un server proxy:
```shell
chromium --proxy-server="{{socks5://hostname:66}}" {{esempio.com}}
```
{% endraw %}