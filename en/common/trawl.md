---
layout: default
title: "trawl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trawl">
  <a href="/en/common/trawl.html">trawl</a> <a href="#trawl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints out network interface information to the console, much like ifconfig/ipconfig/ip/ifdata.
> More information: <https://github.com/robphoenix/trawl>.

#### Show column names:
```shell
trawl -n
```
#### Filter interface names using a case insensitive regular expression:
```shell
trawl -f wi
```
#### Get a list of available interfaces:
```shell
trawl -i
```
#### Include the loopback interface:
```shell
trawl -l
```
{% endraw %}