---
layout: default
title: "prosodyctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="prosodyctl">
  <a href="/en/common/prosodyctl.html">prosodyctl</a> <a href="#prosodyctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The control tool for the Prosody XMPP server.
> More information: <https://prosody.im/doc/prosodyctl>.

#### Show the status of the Prosody server:
```shell
sudo prosodyctl status
```
#### Reload the server's configuration files:
```shell
sudo prosodyctl reload
```
#### Add a user to the Prosody XMPP server:
```shell
sudo prosodyctl adduser {{user@example.com}}
```
#### Set a user's password:
```shell
sudo prosodyctl passwd {{user@example.com}}
```
#### Permanently delete a user:
```shell
sudo prosodyctl deluser {{user@example.com}}
```
{% endraw %}