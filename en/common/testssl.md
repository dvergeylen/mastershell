---
layout: default
title: "testssl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="testssl">
  <a href="/en/common/testssl.html">testssl</a> <a href="#testssl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check SSL/TLS protocols and ciphers supported by a server.
> More information: <https://testssl.sh/>.

#### Test a server (run every check) on port 443:
```shell
testssl {{example.com}}
```
#### Test a different port:
```shell
testssl {{example.com:465}}
```
#### Only check available protocols:
```shell
testssl --protocols {{example.com}}
```
#### Only check vulnerabilities:
```shell
testssl --vulnerable {{example.com}}
```
#### Only check HTTP security headers:
```shell
testssl --headers {{example.com}}
```
{% endraw %}