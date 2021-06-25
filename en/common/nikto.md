---
layout: default
title: "nikto"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nikto">
  <a href="/en/common/nikto.html">nikto</a> <a href="#nikto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web server scanner which performs tests against web servers for multiple items.
> More information: <https://cirt.net/Nikto2>.

#### Perform a basic Nikto scan against a target host:
```shell
perl nikto.pl -h {{192.168.0.1}}
```
#### Specify the port number when performing a basic scan:
```shell
perl nikto.pl -h {{192.168.0.1}} -p {{443}}
```
#### Scan ports and protocols with full URL syntax:
```shell
perl nikto.pl -h {{https://192.168.0.1:443/}}
```
#### Scan multiple ports in the same scanning session:
```shell
perl nikto.pl -h {{192.168.0.1}} -p {{80,88,443}}
```
#### Update to the latest plugins and databases:
```shell
perl nikto.pl -update
```
{% endraw %}