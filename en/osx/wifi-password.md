---
layout: default
title: "wifi-password"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wifi-password">
  <a href="/en/osx/wifi-password.html">wifi-password</a> <a href="#wifi-password"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get the password of the wifi.
> More information: <https://github.com/rauchg/wifi-password>.

#### Get the password for the wifi you are currently logged onto:
```shell
wifi-password
```
#### Get the password for the wifi with a specific SSID:
```shell
wifi-password {{ssid}}
```
#### Print only the password as output:
```shell
wifi-password -q
```
{% endraw %}