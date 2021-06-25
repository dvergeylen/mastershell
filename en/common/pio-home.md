---
layout: default
title: "pio home"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-home">
  <a href="/en/common/pio-home.html">pio home</a> <a href="#pio-home"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Launch the PlatformIO Home web server.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_home.html>.

#### Open PlatformIO Home in the default web browser:
```shell
pio home
```
#### Use a specific HTTP port (defaults to 8008):
```shell
pio home --port {{port}}
```
#### Bind to a specific IP address (defaults to 127.0.0.1):
```shell
pio home --host {{ip_address}}
```
#### Do not automatically open PlatformIO Home in the default web browser:
```shell
pio home --no-open
```
#### Automatically shutdown the server on timeout (in seconds) when no clients are connected:
```shell
pio home --shutdown-timeout {{time}}
```
#### Specify a unique session identifier to keep PlatformIO Home isolated from other instances and protected from 3rd party access:
```shell
pio home --session-id {{id}}
```
{% endraw %}