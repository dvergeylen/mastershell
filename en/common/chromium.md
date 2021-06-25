---
layout: default
title: "chromium"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chromium">
  <a href="/en/common/chromium.html">chromium</a> <a href="#chromium"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open-source web browser from Google.
> More information: <https://chromium.org>.

#### Open a file:
```shell
chromium {{path/to/file.html}}
```
#### Open an URL:
```shell
chromium {{example.com}}
```
#### Open in incognito mode:
```shell
chromium --incognito {{example.com}}
```
#### Open in a new window:
```shell
chromium --new-window {{example.com}}
```
#### Open in app mode (without toolbars, URL bar, buttons, etc.):
```shell
chromium --app='{{https://example.com}}'
```
#### Use a proxy server:
```shell
chromium --proxy-server="{{socks5://hostname:66}}" {{example.com}}
```
{% endraw %}