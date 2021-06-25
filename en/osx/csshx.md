---
layout: default
title: "csshX"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csshx">
  <a href="/en/osx/csshx.html">csshX</a> <a href="#csshx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cluster SSH tool for macOS.
> More information: <https://github.com/brockgr/csshx>.

#### Connect to multiple hosts:
```shell
csshX {{hostname1}} {{hostname2}}
```
#### Connect to multiple hosts with a given SSH key:
```shell
csshX {{user@hostname1}} {{user@hostname2}} '--ssh_args' '-i {{path/to/ssh_key.pem}}'
```
#### Connect to a pre-defined cluster from `/etc/clusters`:
```shell
csshX cluster1
```
{% endraw %}