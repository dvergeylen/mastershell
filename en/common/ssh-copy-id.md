---
layout: default
title: "ssh-copy-id"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-copy-id">
  <a href="/en/common/ssh-copy-id.html">ssh-copy-id</a> <a href="#ssh-copy-id"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install your public key in a remote machine's authorized_keys.

#### Copy your keys to the remote machine:
```shell
ssh-copy-id {{username@remote_host}}
```
#### Copy the given public key to the remote:
```shell
ssh-copy-id -i {{path/to/certificate}} {{username}}@{{remote_host}}
```
#### Copy the given public key to the remote with specific port:
```shell
ssh-copy-id -i {{path/to/certificate}} -p {{port}} {{username}}@{{remote_host}}
```
{% endraw %}