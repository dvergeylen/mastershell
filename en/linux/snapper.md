---
layout: default
title: "snapper"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="snapper">
  <a href="/en/linux/snapper.html">snapper</a> <a href="#snapper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filesystem snapshot management tool.
> More information: <http://snapper.io/manpages/snapper.html>.

#### List snapshot configs:
```shell
snapper list-configs
```
#### Create snapper config:
```shell
snapper -c {{config}} create-config {{path/to/directory}}
```
#### Create a snapshot with a description:
```shell
snapper -c {{config}} create -d "{{snapshot_description}}"
```
#### List snapshots for a config:
```shell
snapper -c {{config}} list
```
#### Delete a snapshot:
```shell
snapper -c {{config}} delete {{snapshot_number}}
```
#### Delete a range of snapshots:
```shell
snapper -c {{config}} delete {{snapshot_X}}-{{snapshot_Y}}
```
{% endraw %}