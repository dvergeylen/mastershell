---
layout: default
title: "duplicity"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="duplicity">
  <a href="/en/common/duplicity.html">duplicity</a> <a href="#duplicity"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates incremental, compressed, encrypted and versioned backups.
> Can also upload the backups to a variety of backend services.
> More information: <http://duplicity.nongnu.org>.

#### Backup a directory via FTPS to a remote machine, encrypting it with a password:
```shell
FTP_PASSWORD={{ftp_login_password}} PASSPHRASE={{encryption_password}} duplicity {{path/to/source/directory}} {{ftps://user@hostname/target/directory/path/}}
```
#### Backup a directory to Amazon S3, doing a full backup every month:
```shell
duplicity --full-if-older-than {{1M}} --use-new-style s3://{{bucket_name[/prefix]}}
```
#### Delete versions older than 1 year from a backup stored on a WebDAV share:
```shell
FTP_PASSWORD={{webdav_login_password}} duplicity remove-older-than {{1Y}} --force {{webdav[s]://user@hostname[:port]/some_dir}}
```
#### List the available backups:
```shell
duplicity collection-status "file://{{absolute/path/to/backup/directory}}"
```
#### List the files in a backup stored on a remote machine, via ssh:
```shell
duplicity list-current-files --time {{YYYY-MM-DD}} scp://{{user@hostname}}/path/to/backup/dir
```
#### Restore a subdirectory from a GnuPG-encrypted local backup to a given location:
```shell
PASSPHRASE={{gpg_key_password}} duplicity restore --encrypt-key {{gpg_key_id}} --file-to-restore {{relative/path/restoredirectory}} file://{{absolute/path/to/backup/directory}} {{path/to/directory/to/restore/to}}
```
{% endraw %}