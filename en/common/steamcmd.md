---
layout: default
title: "steamcmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="steamcmd">
  <a href="/en/common/steamcmd.html">steamcmd</a> <a href="#steamcmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line version of the Steam client.
> More information: <https://manned.org/steamcmd>.

#### Install or update an application anonymously:
```shell
steamcmd +login {{anonymous}} +app_update {{appid}} +quit
```
#### Install or update an application using the specified credentials:
```shell
steamcmd +login {{username}} +app_update {{appid}} +quit
```
#### Install an application for a specific platform:
```shell
steamcmd +@sSteamCmdForcePlatformType {{windows}} +login {{anonymous}} +app_update {{appid}} validate +quit
```
{% endraw %}