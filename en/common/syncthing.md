---
layout: default
title: "syncthing"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="syncthing">
  <a href="/en/common/syncthing.html">syncthing</a> <a href="#syncthing"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Continuous bidirectional decentralised folder synchronisation tool.
> More information: <https://docs.syncthing.net/>.

#### Start syncthing:
```shell
syncthing
```
#### Start syncthing without opening a web browser:
```shell
syncthing -no-browser
```
#### Print the device ID:
```shell
syncthing -device-id
```
#### Change the home directory:
```shell
syncthing -home={{path/to/directory}}
```
#### Force a full index exchange:
```shell
syncthing -reset-deltas
```
#### Change the address upon which the web interface listens:
```shell
syncthing -gui-address={{ip_address:port|path/to/socket.sock}}
```
#### Show filepaths to the files used by syncthing:
```shell
syncthing -paths
```
#### Disable the syncthing monitor process:
```shell
syncthing -no-restart
```
{% endraw %}