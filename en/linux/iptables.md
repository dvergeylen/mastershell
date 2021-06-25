---
layout: default
title: "iptables"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iptables">
  <a href="/en/linux/iptables.html">iptables</a> <a href="#iptables"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Program that allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> More information: <https://www.netfilter.org/projects/iptables/>.

#### View chains, rules, and packet/byte counters for the filter table:
```shell
sudo iptables -vnL
```
#### Set chain policy rule:
```shell
sudo iptables -P {{chain}} {{rule}}
```
#### Append rule to chain policy for IP:
```shell
sudo iptables -A {{chain}} -s {{ip}} -j {{rule}}
```
#### Append rule to chain policy for IP considering protocol and port:
```shell
sudo iptables -A {{chain}} -s {{ip}} -p {{protocol}} --dport {{port}} -j {{rule}}
```
#### Delete chain rule:
```shell
sudo iptables -D {{chain}} {{rule_line_number}}
```
#### Save iptables configuration of a given table to a file:
```shell
sudo iptables-save -t {{tablename}} > {{path/to/iptables_file}}
```
#### Restore iptables configuration from a file:
```shell
sudo iptables-restore < {{path/to/iptables_file}}
```
{% endraw %}