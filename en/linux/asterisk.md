---
layout: default
title: "asterisk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asterisk">
  <a href="/en/linux/asterisk.html">asterisk</a> <a href="#asterisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Telephone and exchange (phone) server.
> Used for running the server itself, and managing an already running instance.
> More information: <https://wiki.asterisk.org/wiki/display/AST/Home>.

#### [R]econnect to a running server, and turn on logging 3 levels of [v]erbosity:
```shell
asterisk -r -vvv
```
#### [R]econnect to a running server, run a single command, and return:
```shell
asterisk -r -x "{{command}}"
```
#### Show chan_SIP clients (phones):
```shell
asterisk -r -x "sip show peers"
```
#### Show active calls and channels:
```shell
asterisk -r -x "core show channels"
```
#### Show voicemail mailboxes:
```shell
asterisk -r -x "voicemail show users"
```
#### Terminate a channel:
```shell
asterisk -r -x "hangup request {{channel_ID}}"
```
#### Reload chan_SIP configuration:
```shell
asterisk -r -x "sip reload"
```
{% endraw %}