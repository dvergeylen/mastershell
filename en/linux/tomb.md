---
layout: default
title: "tomb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tomb">
  <a href="/en/linux/tomb.html">tomb</a> <a href="#tomb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage encrypted storage directories that can be safely transported and hidden in a filesystem.
> More information: <https://www.dyne.org/software/tomb/>.

#### Create a new tomb with an initial size of 100MB:
```shell
tomb dig -s {{100}} {{encrypted_directory.tomb}}
```
#### Create a new key file that can be used to lock a tomb; user will be prompted for a password for the key:
```shell
tomb forge {{encrypted_directory.tomb.key}}
```
#### Initialize and lock an empty tomb using a key made with `forge`:
```shell
tomb lock {{encrypted_directory.tomb}} -k {{encrypted_directory.tomb.key}}
```
#### Mount a tomb (by default in `/media`) using its key, making it usable as a regular filesystem directory:
```shell
tomb open {{encrypted_directory.tomb}} -k {{encrypted_directory.tomb.key}}
```
#### Close a tomb (fails if the tomb is being used by a process):
```shell
tomb close {{encrypted_directory.tomb}}
```
#### Forcefully close all open tombs, killing any applications using them:
```shell
tomb slam all
```
#### List all open tombs:
```shell
tomb list
```
{% endraw %}