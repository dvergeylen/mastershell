---
layout: default
title: "ntpq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ntpq">
  <a href="/en/linux/ntpq.html">ntpq</a> <a href="#ntpq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the Network Time Protocol (NTP) daemon.
> More information: <https://www.eecis.udel.edu/~mills/ntp/html/ntpq.html>.

#### Start `ntpq` in interactive mode:
```shell
ntpq --interactive
```
#### Print a list of NTP peers:
```shell
ntpq --peers
```
#### Print a list of NTP peers without resolving hostnames from IP addresses:
```shell
ntpq --numeric --peers
```
#### Use `ntpq` in debugging mode:
```shell
ntpq --debug-level
```
#### Print NTP system variables values:
```shell
ntpq --command={{rv}}
```
{% endraw %}