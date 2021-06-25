---
layout: default
title: "airport"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airport">
  <a href="/en/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wireless network configuration utility.

#### Show current wireless status information:
```shell
airport -I
```
#### Sniff wireless traffic on channel 1:
```shell
airport sniff {{1}}
```
#### Scan for available wireless networks:
```shell
airport -s
```
#### Disassociate from current airport network:
```shell
sudo airport -z
```
{% endraw %}