---
layout: default
title: "dbus-daemon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dbus-daemon">
  <a href="/en/linux/dbus-daemon.html">dbus-daemon</a> <a href="#dbus-daemon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The D-Bus message daemon, allowing multiple programs to exchange messages.

#### Run the daemon with a configuration file:
```shell
dbus-daemon --config-file {{path/to/file}}
```
#### Run the daemon with the standard per-login-session message bus configuration:
```shell
dbus-daemon --session
```
#### Run the daemon with the standard systemwide message bus configuration:
```shell
dbus-daemon --system
```
#### Set the address to listen on and override the configuration value for it:
```shell
dbus-daemon --address {{address}}
```
#### Output the process id to stdout:
```shell
dbus-daemon --print-pid
```
#### Force the message bus to write to the system log for messages:
```shell
dbus-daemon --syslog
```
{% endraw %}