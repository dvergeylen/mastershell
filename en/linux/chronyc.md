---
layout: default
title: "chronyc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chronyc">
  <a href="/en/linux/chronyc.html">chronyc</a> <a href="#chronyc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the Chrony NTP daemon.
> More information: <https://chrony.tuxfamily.org/doc/4.0/chronyc.html>.

#### Start chronyc in interactive mode:
```shell
chronyc
```
#### Display tracking stats for the Chrony daemon:
```shell
chronyc tracking
```
#### Print the time sources that Chrony is currently using:
```shell
chronyc sources
```
#### Display stats for sources currently used by chrony daemon as a time source:
```shell
chronyc sourcestats
```
#### Step the system clock immediately, bypassing any slewing:
```shell
chronyc makestep
```
#### Display verbose information about each NTP source:
```shell
chronyc ntpdata
```
{% endraw %}