---
layout: default
title: "salt-call"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="salt-call">
  <a href="/en/common/salt-call.html">salt-call</a> <a href="#salt-call"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Invoke salt locally on a salt minion.
> More information: <https://docs.saltstack.com/ref/cli/salt-call.html>.

#### Perform a highstate on this minion:
```shell
salt-call state.highstate
```
#### Perform a highstate dry-run, compute all changes but don't actually perform them:
```shell
salt-call state.highstate test=true
```
#### Perform a highstate with verbose debugging output:
```shell
salt-call -l debug state.highstate
```
#### List this minion's grains:
```shell
salt-call grains.items
```
{% endraw %}