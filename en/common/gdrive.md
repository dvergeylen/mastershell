---
layout: default
title: "gdrive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gdrive">
  <a href="/en/common/gdrive.html">gdrive</a> <a href="#gdrive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to interact with Google Drive.
> Folder/file id can be obtained from the Google Drive folder or id url.
> More information: <https://github.com/gdrive-org/gdrive>.

#### Upload a local path to the parent folder with the specified id:
```shell
gdrive upload -p {{id}} {{path/to/file_or_folder}}
```
#### Download file or directory by id to current directory:
```shell
gdrive download {{id}}
```
#### Download to a given local path by its id:
```shell
gdrive download --path {{path/to/folder}} {{id}}
```
#### Create a new revision of an id using a given file or folder:
```shell
gdrive update {{id}} {{path/to/file_or_folder}}
```
{% endraw %}