---
layout: default
title: "mosquitto_passwd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mosquitto_passwd">
  <a href="/en/common/mosquitto_passwd.html">mosquitto_passwd</a> <a href="#mosquitto_passwd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage password files for mosquitto.
> See also `mosquitto`, the MQTT server that this manages.
> More information: <https://mosquitto.org/man/mosquitto_passwd-1.html>.

#### Add a new user to a password file (will prompt to enter the password):
```shell
mosquitto_passwd {{path/to/password_file}} {{username}}
```
#### Create the password file if it doesn't already exist:
```shell
mosquitto_passwd -c {{path/to/password_file}} {{username}}
```
#### Delete the specified username instead:
```shell
mosquitto_passwd -D {{path/to/password_file}} {{username}}
```
#### Upgrade an old plain-text password file to a hashed password file:
```shell
mosquitto_passwd -U {{path/to/password_file}}
```
{% endraw %}