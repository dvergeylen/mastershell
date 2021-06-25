---
layout: default
title: "skicka"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="skicka">
  <a href="/en/common/skicka.html">skicka</a> <a href="#skicka"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage your Google Drive.
> More information: <https://github.com/google/skicka>.

#### Upload a file/folder to Google Drive:
```shell
skicka upload {{path/to/local}} {{path/to/remote}}
```
#### Download a file/folder from Google Drive:
```shell
skicka download {{path/to/remote}} {{path/to/local}}
```
#### List files:
```shell
skicka ls {{path/to/folder}}
```
#### Show amount of space used by children folders:
```shell
skicka du {{path/to/parent/folder}}
```
#### Create a folder:
```shell
skicka mkdir {{path/to/folder}}
```
#### Delete a file:
```shell
skicka rm {{path/to/file}}
```
{% endraw %}