---
layout: default
title: "rusnapshot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rusnapshot">
  <a href="/en/linux/rusnapshot.html">rusnapshot</a> <a href="#rusnapshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> BTRFS snapshotting utility written in Rust.
> More information: <https://github.com/Edu4rdSHL/rusnapshot>.

#### Create a snapshot using a config file:
```shell
sudo rusnapshot --config {{path/to/config.toml}} --cr
```
#### List created snapshots:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --list
```
#### Delete a snapshot by ID or the name of the snapshot:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --del --id {{snapshot_id}}
```
#### Delete all `hourly` snapshots:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --list --keep {{0}} --clean --kind {{hourly}}
```
#### Create a read-write snapshot:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --cr --rw
```
#### Restore a snapshot:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --id {{snapshot_id}} --restore
```
{% endraw %}