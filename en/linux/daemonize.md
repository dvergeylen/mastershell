---
layout: default
title: "daemonize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="daemonize">
  <a href="/en/linux/daemonize.html">daemonize</a> <a href="#daemonize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command (that does not daemonize itself) as a Unix daemon.
> More information: <http://software.clapper.org/daemonize/>.

#### Run a command as a daemon:
```shell
daemonize {{command}} {{command_arguments}}
```
#### Write the pid to the specified file:
```shell
daemonize -p {{path/to/pidfile}} {{command}} {{command_arguments}}
```
#### Use a lock file to ensure that only one instance runs at a time:
```shell
daemonize -l {{path/to/lockfile}} {{command}} {{command_arguments}}
```
#### Use the specified user account:
```shell
sudo daemonize -u {{user}} {{command}} {{command_arguments}}
```
{% endraw %}