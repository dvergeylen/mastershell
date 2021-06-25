---
layout: default
title: "runcon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runcon">
  <a href="/en/linux/runcon.html">runcon</a> <a href="#runcon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a program in a different SELinux security context.
> With neither context nor command, print the current security context.
> More information: <https://www.gnu.org/software/coreutils/runcon>.

#### Determine the current domain:
```shell
runcon
```
#### Specify the domain to run a command in:
```shell
runcon -t {{domain}}_t {{command}}
```
#### Specify the context role to run a command with:
```shell
runcon -r {{role}}_r {{command}}
```
#### Specify the full context to run a command with:
```shell
runcon {{user}}_u:{{role}}_r:{{domain}}_t {{command}}
```
{% endraw %}