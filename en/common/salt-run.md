---
layout: default
title: "salt-run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="salt-run">
  <a href="/en/common/salt-run.html">salt-run</a> <a href="#salt-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Frontend for executing salt-runners on minions.
> More information: <https://docs.saltstack.com/ref/cli/salt-run.html>.

#### Show status of all minions:
```shell
salt-run manage.status
```
#### Show all minions which are disconnected:
```shell
salt-run manage.up
```
{% endraw %}