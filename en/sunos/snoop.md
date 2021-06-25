---
layout: default
title: "snoop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="snoop">
  <a href="/en/sunos/snoop.html">snoop</a> <a href="#snoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Network packet sniffer.
> SunOS equivalent of tcpdump.
> More information: <https://www.unix.com/man-page/sunos/1m/snoop>.

#### Capture packets on a specific network interface:
```shell
snoop -d {{e1000g0}}
```
#### Save captured packets in a file instead of displaying them:
```shell
snoop -o {{filename}}
```
#### Display verbose protocol layer summary of packets from a file:
```shell
snoop -V -i {{filename}}
```
#### Capture network packets that come from a hostname and go to a given port:
```shell
snoop to port {{port}} from host {{hostname}}
```
#### Capture and show an hex-dump of network packets exchanged between two IP addresses:
```shell
snoop -x0 -p4 {{ip_address_1}} {{ip_address_2}}
```
{% endraw %}