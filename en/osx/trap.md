---
layout: default
title: "trap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trap">
  <a href="/en/osx/trap.html">trap</a> <a href="#trap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automatically execute commands after receiving signals by processes or the operating system.
> Can be used to perform cleanups for interruptions by the user or other actions.

#### List available signals to set traps for:
```shell
trap -l
```
#### List active traps for the current shell:
```shell
trap -p
```
#### Set a trap to execute commands when one or more signals are detected:
```shell
trap 'echo "Caught signal {{SIGHUP}}"' {{SIGHUP}}
```
#### Remove active traps:
```shell
trap - {{SIGHUP}} {{SIGINT}}
```
{% endraw %}