---
layout: default
title: "apk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apk">
  <a href="/en/linux/apk.html">apk</a> <a href="#apk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alpine Linux package management tool.

#### Update repository indexes from all remote repositories:
```shell
apk update
```
#### Install a new package:
```shell
apk add {{package}}
```
#### Remove a package:
```shell
apk del {{package}}
```
#### Repair package or upgrade it without modifying main dependencies:
```shell
apk fix {{package}}
```
#### Search package via keyword:
```shell
apk search {{keyword}}
```
#### Get info about a specific package:
```shell
apk info {{package}}
```
{% endraw %}