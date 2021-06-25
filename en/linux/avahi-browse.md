---
layout: default
title: "avahi-browse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="avahi-browse">
  <a href="/en/linux/avahi-browse.html">avahi-browse</a> <a href="#avahi-browse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays services and hosts exposed on the local network via mDNS/DNS-SD.
> Avahi is compatible with Bonjour (Zeroconf) found in Apple devices.
> More information: <https://www.avahi.org/>.

#### List all services available on the local network along with their addresses and ports while ignoring local ones:
```shell
avahi-browse --all --resolve --ignore-local
```
#### List all domains:
```shell
avahi-browse --browse-domains
```
#### Limit the search to a particular domain:
```shell
avahi-browse --all --domain={{domain}}
```
{% endraw %}