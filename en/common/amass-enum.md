---
layout: default
title: "amass enum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amass-enum">
  <a href="/en/common/amass-enum.html">amass enum</a> <a href="#amass-enum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find subdomains of a domain.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-enum-subcommand>.

#### Passively find subdomains of a domain:
```shell
amass enum -passive -d {{domain_name}}
```
#### Find subdomains of a domain and actively verify them attempting to resolve the found subdomains:
```shell
amass enum -active -d {{domain_name}} -p {{80,443,8080}}
```
#### Do a brute force search for subdomains:
```shell
amass enum -brute -d {{domain_name}}
```
#### Save the results to a text file:
```shell
amass enum -o {{output_file}} -d {{domain_name}}
```
#### Save the results to a database:
```shell
amass enum -o {{output_file}} -dir {{path/to/database_directory}}
```
{% endraw %}