---
layout: default
title: "irssi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="irssi">
  <a href="/en/common/irssi.html">irssi</a> <a href="#irssi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Text based IRC client.
> More information: <https://irssi.org>.

#### Open irssi and connect to a server with a nickname:
```shell
irssi -n {{nickname}} -c {{irc.example.com}}
```
#### Open irssi and connect with a specific server on a given port:
```shell
irssi -c {{irc.example.com}} -p {{port}}
```
#### View the help:
```shell
irssi --help
```
#### Join a channel:
```shell
/join {{#channelname}}
```
#### Change active window (starts at 1):
```shell
/win {{window_number}}
```
#### Exit the application cleanly and quitting any server(s):
```shell
/quit
```
{% endraw %}