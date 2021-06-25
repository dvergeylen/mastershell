---
layout: default
title: "pihole"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pihole">
  <a href="/en/linux/pihole.html">pihole</a> <a href="#pihole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal interface for the Pi-Hole ad-blocking DNS server.
> More information: <https://pi-hole.net>.

#### Check the Pi-hole daemon's status:
```shell
pihole status
```
#### Monitor detailed system status:
```shell
pihole chronometer
```
#### Start or stop the daemon:
```shell
pihole {{enable|disable}}
```
#### Restart the daemon (not the server itself):
```shell
pihole restartdns
```
#### Whitelist or blacklist a domain:
```shell
pihole {{whitelist|blacklist}} {{example.com}}
```
#### Search the lists for a domain:
```shell
pihole query {{example.com}}
```
{% endraw %}