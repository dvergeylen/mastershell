---
layout: default
title: "ssh-add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-add">
  <a href="/en/linux/ssh-add.html">ssh-add</a> <a href="#ssh-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage loaded ssh keys in the ssh-agent.
> Ensure that ssh-agent is up and running for the keys to be loaded in it.

#### Add the default ssh keys in `~/.ssh` to the ssh-agent:
```shell
ssh-add
```
#### Add a specific key to the ssh-agent:
```shell
ssh-add {{path/to/private_key}}
```
#### List fingerprints of currently loaded keys:
```shell
ssh-add -l
```
#### Delete a key from the ssh-agent:
```shell
ssh-add -d {{path/to/private_key}}
```
#### Delete all currently loaded keys from the ssh-agent:
```shell
ssh-add -D
```
{% endraw %}