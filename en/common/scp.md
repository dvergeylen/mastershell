---
layout: default
title: "scp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scp">
  <a href="/en/common/scp.html">scp</a> <a href="#scp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Secure copy.
> Copy files between hosts using Secure Copy Protocol over SSH.
> More information: <https://man.openbsd.org/scp>.

#### Copy a local file to a remote host:
```shell
scp {{path/to/local_file}} {{remote_host}}:{{path/to/remote_file}}
```
#### Use a specific port when connecting to the remote host:
```shell
scp -P {{port}} {{path/to/local_file}} {{remote_host}}:{{path/to/remote_file}}
```
#### Copy a file from a remote host to a local directory:
```shell
scp {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}
```
#### Recursively copy the contents of a directory from a remote host to a local directory:
```shell
scp -r {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}
```
#### Copy a file between two remote hosts transferring through the local host:
```shell
scp -3 {{host1}}:{{path/to/remote_file}} {{host2}}:{{path/to/remote_directory}}
```
#### Use a specific username when connecting to the remote host:
```shell
scp {{path/to/local_file}} {{remote_username}}@{{remote_host}}:{{path/to/remote_directory}}
```
#### Use a specific ssh private key for authentication with the remote host:
```shell
scp -i {{~/.ssh/private_key}} {{local_file}} {{remote_host}}:{{/path/remote_file}}
```
{% endraw %}