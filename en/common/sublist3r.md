---
layout: default
title: "sublist3r"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sublist3r">
  <a href="/en/common/sublist3r.html">sublist3r</a> <a href="#sublist3r"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fast subdomains enumeration tool for penetration testers.
> More information: <https://github.com/aboul3la/Sublist3r>.

#### Find subdomains for a domain:
```shell
sublist3r --domain {{domain_name}}
```
#### Find subdomains for a domain, also enabling brute force search:
```shell
sublist3r --domain {{domain_name}} --bruteforce
```
#### Save the found subdomains to a text file:
```shell
sublist3r --domain {{domain_name}} --output {{path/to/output_file}}
```
#### Output all available options:
```shell
sublist3r --help
```
{% endraw %}