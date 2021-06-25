---
layout: default
title: "mmcli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mmcli">
  <a href="/en/linux/mmcli.html">mmcli</a> <a href="#mmcli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control and monitor the ModemManager.
> More information: <https://www.freedesktop.org/software/ModemManager/man/latest/mmcli.1.html>.

#### List SMS messages available on the modem:
```shell
sudo mmcli --modem={{modem}} --messaging-list-sms
```
#### Delete a message from the modem, specifying its path:
```shell
sudo mmcli --modem={{modem}} --messaging-delete-sms={{path/to/message_file}}
```
{% endraw %}