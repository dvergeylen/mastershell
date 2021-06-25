---
layout: default
title: "airpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airpaste">
  <a href="/en/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Share messages and files on the same network using mDNS.
> More information: <https://github.com/mafintosh/airpaste>.

#### Wait for a message and display it when received:
```shell
airpaste
```
#### Send text:
```shell
echo {{text}} | airpaste
```
#### Send a file:
```shell
airpaste < {{path/to/file}}
```
#### Receive a file:
```shell
airpaste > {{path/to/file}}
```
#### Create or join a channel:
```shell
airpaste {{channel_name}}
```
{% endraw %}