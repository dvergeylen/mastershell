---
layout: default
title: "salt-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="salt-key">
  <a href="/en/common/salt-key.html">salt-key</a> <a href="#salt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manages salt minion keys on the salt master.
> Needs to be run on the salt master, likely as root or with sudo.
> More information: <https://docs.saltstack.com/ref/cli/salt-key.html>.

#### List all accepted, unaccepted and rejected minion keys:
```shell
salt-key -L
```
#### Accept a minion key by name:
```shell
salt-key -a {{MINION_ID}}
```
#### Reject a minion key by name:
```shell
salt-key -r {{MINION_ID}}
```
#### Print fingerprints of all public keys:
```shell
salt-key -F
```
{% endraw %}