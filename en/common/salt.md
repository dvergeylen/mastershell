---
layout: default
title: "salt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="salt">
  <a href="/en/common/salt.html">salt</a> <a href="#salt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute commands and assert state on remote salt minions.
> More information: <https://docs.saltstack.com/ref/cli/salt.html>.

#### List connected minions:
```shell
salt '*' test.ping
```
#### Execute a highstate on all connected minions:
```shell
salt '*' state.highstate
```
#### Upgrade packages using the OS package manager (apt, yum, brew) on a subset of minions:
```shell
salt '*.example.com' pkg.upgrade
```
#### Execute an arbitrary command on a particular minion:
```shell
salt '{{minion_id}}' cmd.run "ls "
```
{% endraw %}