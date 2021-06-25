---
layout: default
title: "microcom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="microcom">
  <a href="/en/linux/microcom.html">microcom</a> <a href="#microcom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A minimalistic terminal program, used to access remote devices via a serial, CAN or telnet connection from the console.

#### Open a serial port using the specified baud rate:
```shell
microcom --port {{path/to/serial_port}} --speed {{baud_rate}}
```
#### Establish a telnet connection to the specified host:
```shell
microcom --telnet {{hostname}}:{{port}}
```
{% endraw %}