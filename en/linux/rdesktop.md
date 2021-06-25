---
layout: default
title: "rdesktop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rdesktop">
  <a href="/en/linux/rdesktop.html">rdesktop</a> <a href="#rdesktop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remote Desktop Protocol client.
> It can be used to connect the remote computer using the RDP protocol.

#### Connect to a remote computer (default port is 3389):
```shell
rdesktop -u {{username}} -p {{password}} {{host:port}}
```
#### Simple Examples:
```shell
rdesktop -u Administrator -p passwd123 192.168.1.111:3389
```
#### Connect to a remote computer with full screen (press `Ctrl + Alt + Enter` to exist):
```shell
rdesktop -u {{username}} -p {{password}} -f {{host:port}}
```
#### Use the customed resolution (use the letter 'x' between the number):
```shell
rdesktop -u {{username}} -p {{password}} -g 1366x768 {{host:port}}
```
#### Connect to a remote computer using domain user:
```shell
rdesktop -u {{username}} -p {{password}} -d {{domainname}} {{host:port}}
```
#### Use the 16 bit color (speed up):
```shell
rdesktop -u {{username}} -p {{password}} -a 16 {{host:port}}
```
{% endraw %}