---
layout: default
title: "veracrypt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="veracrypt">
  <a href="/en/linux/veracrypt.html">veracrypt</a> <a href="#veracrypt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Free and open source disk encryption software.
> More information: <https://www.veracrypt.fr/code/VeraCrypt/plain/doc/html/Documentation.html>.

#### Create a new volume through a text user interface and use `/dev/urandom` as a source of random data:
```shell
veracrypt --text --create --random-source={{/dev/urandom}}
```
#### Decrypt a volume interactively through a text user interface and mount it to a directory:
```shell
veracrypt --text {{path/to/volume}} {{path/to/mount_point}}
```
#### Decrypt a partition using a keyfile and mount it to a directory:
```shell
veracrypt --keyfiles={{path/to/keyfile}} {{/dev/sdXN}} {{path/to/mount_point}}
```
#### Dismount a volume on the directory it is mounted to:
```shell
veracrypt --dismount {{path/to/mounted_point}}
```
{% endraw %}