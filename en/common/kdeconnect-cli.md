---
layout: default
title: "kdeconnect-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kdeconnect-cli">
  <a href="/en/common/kdeconnect-cli.html">kdeconnect-cli</a> <a href="#kdeconnect-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE Connect CLI.
> More information: <https://kdeconnect.kde.org>.

#### List all devices:
```shell
kdeconnect-cli --list-devices
```
#### List available (paired and reachable) devices:
```shell
kdeconnect-cli --list-available
```
#### Request pairing with a specific device, specifying its ID:
```shell
kdeconnect-cli --pair --device {{device_id}}
```
#### Ring a device, specifying its name:
```shell
kdeconnect-cli --ring --name {{device_name}}
```
#### Share an URL or file with a paired device, specifying its ID:
```shell
kdeconnect-cli --share {{URL|path/to/file}} --device {{device_id}}
```
#### Send an SMS with an optional attachment to a specific number:
```shell
kdeconnect-cli --name {{device_name}} --send-sms {{message}} --destination {{phone_number}} --attachment {{path/to/file}}
```
#### Unlock a specific device:
```shell
kdeconnect-cli --name {{device_name}} --unlock
```
#### Simulate a key press on a specific device:
```shell
kdeconnect-cli --name {{device_name}} --send-keys {{key}}
```
{% endraw %}