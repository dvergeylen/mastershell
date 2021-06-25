---
layout: default
title: "subfinder"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="subfinder">
  <a href="/en/common/subfinder.html">subfinder</a> <a href="#subfinder"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A subdomain discovery tool that discovers valid subdomains for websites.
> Designed as a passive framework to be useful for bug bounties and safe for penetration testing.
> More information: <https://github.com/subfinder/subfinder>.

#### Find subdomains for a specific domain:
```shell
subfinder -d {{example.com}}
```
#### Show only the subdomains found:
```shell
subfinder --silent -d {{example.com}}
```
#### Use a brute-force attack to find subdomains:
```shell
subfinder -d {{example.com}} -b
```
#### Remove wildcard subdomains:
```shell
subfinder -nW -d {{example.com}}
```
#### Use a given comma-separated list of resolvers:
```shell
subfinder -r {{8.8.8.8}},{{1.1.1.1}} -d {{example.com}}
```
{% endraw %}