---
layout: default
title: "fail2ban-client"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fail2ban-client">
  <a href="/en/linux/fail2ban-client.html">fail2ban-client</a> <a href="#fail2ban-client"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure and control fail2ban server.
> More information: <https://github.com/fail2ban/fail2ban>.

#### Retrieve current status of the jail service:
```shell
fail2ban-client status {{jail}}
```
#### Remove the specified IP from the jail service's ban list:
```shell
fail2ban-client set {{jail}} unbanip {{ip}}
```
#### Verify fail2ban server is alive:
```shell
fail2ban-client ping
```
{% endraw %}