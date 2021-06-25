---
layout: default
title: "rtmpdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rtmpdump">
  <a href="/en/common/rtmpdump.html">rtmpdump</a> <a href="#rtmpdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to dump media content streamed over the RTMP protocol.
> More information: <http://rtmpdump.mplayerhq.hu/>.

#### Download a file:
```shell
rtmpdump --rtmp {{rtmp://example.com/path/to/video}} -o {{file.ext}}
```
#### Download a file from a Flash player:
```shell
rtmpdump --rtmp {{rtmp://example.com/path/to/video}} --swfVfy {{http://example.com/player}} --flashVer "{{LNX 10,0,32,18}}" -o {{file.ext}}
```
#### Specify connection parameters if they are not detected correctly:
```shell
rtmpdump --rtmp {{rtmp://example.com/path/to/video}} --app {{app_name}} --playpath {{path/to/video}} -o {{file.ext}}
```
#### Download a file from a server that requires a referrer:
```shell
rtmpdump --rtmp {{rtmp://example.com/path/to/video}} --pageUrl {{http://example.com/webpage}} -o {{file.ext}}
```
{% endraw %}