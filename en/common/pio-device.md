---
layout: default
title: "pio device"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-device">
  <a href="/en/common/pio-device.html">pio device</a> <a href="#pio-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage and monitor PlatformIO devices.
> More information: <https://docs.platformio.org/en/latest/core/userguide/device/>.

#### List all available serial ports:
```shell
pio device list
```
#### List all available logical devices:
```shell
pio device list --logical
```
#### Start an interactive device monitor:
```shell
pio device monitor
```
#### Start an interactive device monitor and listen to a specific port:
```shell
pio device monitor --port {{/dev/ttyUSBX}}
```
#### Start an interactive device monitor and set a specific baud rate (defaults to 9600):
```shell
pio device monitor --baud {{57600}}
```
#### Start an interactive device monitor and set a specific EOL character (defaults to `CRLF`):
```shell
pio device monitor --eol {{CRLF|CR|LF}}
```
#### Go to the menu of the interactive device monitor:
```shell
Ctrl + T
```
{% endraw %}