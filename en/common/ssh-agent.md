---
layout: default
title: "ssh-agent"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-agent">
  <a href="/en/common/ssh-agent.html">ssh-agent</a> <a href="#ssh-agent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Spawn an SSH Agent process.
> An SSH Agent holds SSH keys decrypted in memory until removed or the process is killed.
> See also `ssh-add`, which can add and manage keys held by an SSH Agent.

#### Start an SSH Agent for the current shell:
```shell
eval $(ssh-agent)
```
#### Kill the currently running agent:
```shell
ssh-agent -k
```
{% endraw %}