---
layout: default
title: "ngrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ngrep">
  <a href="/en/common/ngrep.html">ngrep</a> <a href="#ngrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filter network traffic packets using regular expressions.
> More information: <https://github.com/jpr5/ngrep>.

#### Capture traffic of all interfaces:
```shell
ngrep -d any
```
#### Capture traffic of a specific interface:
```shell
ngrep -d {{eth0}}
```
#### Capture traffic crossing port 22 of interface eth0:
```shell
ngrep -d {{eth0}} port {{22}}
```
#### Capture traffic from or to a host:
```shell
ngrep host {{www.example.com}}
```
#### Filter keyword 'User-Agent:' of interface eth0:
```shell
ngrep -d {{eth0}} '{{User-Agent:}}'
```
{% endraw %}