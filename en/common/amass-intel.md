---
layout: default
title: "amass intel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amass-intel">
  <a href="/en/common/amass-intel.html">amass intel</a> <a href="#amass-intel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Collect open source intel on an organisation like root domains and ASNs.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-intel-subcommand>.

#### Find root domains in an IP address range:
```shell
amass intel -addr {{192.168.0.1-254}}
```
#### Use active recon methods:
```shell
amass intel -active -addr {{192.168.0.1-254}}
```
#### Find root domains related to a domain:
```shell
amass intel -whois -d {{domain_name}}
```
#### Find ASNs belonging to an organisation:
```shell
amass intel -org {{organisation_name}}
```
#### Find root domains belonging to a given Autonomous System Number:
```shell
amass intel -asn {{asn}}
```
#### Save results to a text file:
```shell
amass intel -o {{output_file}} -whois -d {{domain_name}}
```
{% endraw %}