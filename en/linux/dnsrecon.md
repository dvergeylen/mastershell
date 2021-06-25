---
layout: default
title: "dnsrecon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dnsrecon">
  <a href="/en/linux/dnsrecon.html">dnsrecon</a> <a href="#dnsrecon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DNS enumeration tool.
> More information: <https://github.com/darkoperator/dnsrecon>.

#### Scan a domain and save the results to a SQLite database:
```shell
dnsrecon --domain {{example.com}} --db {{path/to/database.sqlite}}
```
#### Scan a domain, specifying the nameserver and performing a zone transfer:
```shell
dnsrecon --domain {{example.com}} --name_server {{nameserver.example.com}} --type axfr
```
#### Scan a domain, using a brute-force attack and a dictionary of subdomains and hostnames:
```shell
dnsrecon --domain {{example.com}} --dictionary {{path/to/dictionary.txt}} --type brt
```
#### Scan a domain, performing a reverse lookup of IP ranges from the SPF record and saving the results to a JSON file:
```shell
dnsrecon --domain {{example.com}} -s --json
```
#### Scan a domain, performing a Google enumeration and saving the results to a CSV file:
```shell
dnsrecon --domain {{example.com}} -g --csv
```
#### Scan a domain, performing DNS cache snooping:
```shell
dnsrecon --domain {{example.com}} --type snoop --name_server {{nameserver.example.com}} --dictionary {{path/to/dictionary.txt}}
```
#### Scan a domain, performing zone walking:
```shell
dnsrecon --domain {{example.com}} --type zonewalk
```
{% endraw %}