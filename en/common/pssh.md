---
layout: default
title: "pssh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pssh">
  <a href="/en/common/pssh.html">pssh</a> <a href="#pssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Parallel SSH program.

#### Run a command on two hosts, and print its output on each server inline:
```shell
pssh -i -H "{{host1}} {{host2}}" {{hostname -i}}
```
#### Run a command and save the output to separate files:
```shell
pssh -H {{host1}} -H {{host2}} -o {{path/to/output_dir}} {{hostname -i}}
```
#### Run a command on multiple hosts, specified in a new-line separated file:
```shell
pssh -i -h {{path/to/hosts_file}} {{hostname -i}}
```
#### Run a command as root (this asks for the root password):
```shell
pssh -i -h {{path/to/hosts_file}} -A -l {{root_username}} {{hostname -i}}
```
#### Run a command with extra SSH arguments:
```shell
pssh -i -h {{path/to/hosts_file}} -x "{{-O VisualHostKey=yes}}" {{hostname -i}}
```
#### Run a command limiting the number of parallel connections to 10:
```shell
pssh -i -h {{path/to/hosts_file}} -p {{10}} '{{cd dir; ./script.sh; exit}}'
```
{% endraw %}