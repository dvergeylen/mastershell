---
layout: default
title: "phar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phar">
  <a href="/en/linux/phar.html">phar</a> <a href="#phar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, update or extract PHP archives (PHAR).

#### Add space-separated files or directories to a Phar file:
```shell
phar add -f {{path/to/phar_file}} {{files_or_directories}}
```
#### Display the contents of a Phar file:
```shell
phar list -f {{path/to/phar_file}}
```
#### Delete the specified file or directory from a Phar file:
```shell
phar delete -f {{path/to/phar_file}} -e {{file_or_directory}}
```
#### Display full usage information and available hashing/compression algorithms:
```shell
phar help
```
#### Compress or uncompress files and directories in a Phar file:
```shell
phar compress -f {{path/to/phar_file}} -c {{algorithm}}
```
#### Get information about a Phar file:
```shell
phar info -f {{path/to/phar_file}}
```
#### Sign a Phar file with a specific hash algorithm:
```shell
phar sign -f {{path/to/phar_file}} -h {{algorithm}}
```
#### Sign a Phar file with an OpenSSL private key:
```shell
phar sign -f {{path/to/phar_file}} -h openssl -y {{path/to/private_key}}
```
{% endraw %}