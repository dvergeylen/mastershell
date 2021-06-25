---
layout: default
title: "distccd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="distccd">
  <a href="/en/common/distccd.html">distccd</a> <a href="#distccd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Server daemon for the distcc distributed compiler.
> More information: <https://distcc.github.io>.

#### Start a daemon with the default settings:
```shell
distccd --daemon
```
#### Start a daemon, accepting connections from IPv4 private network ranges:
```shell
distccd --daemon --allow-private
```
#### Start a daemon, accepting connections from a specific network address or address range:
```shell
distccd --daemon --allow {{ip_address|network_prefix}}
```
#### Start a daemon with a lowered priority that can run a maximum of 4 tasks at a time:
```shell
distccd --daemon --jobs {{4}} --nice {{5}}
```
#### Start a daemon and register it via mDNS/DNS-SD (Zeroconf):
```shell
distccd --daemon --zeroconf
```
{% endraw %}