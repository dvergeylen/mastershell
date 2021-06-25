---
layout: default
title: "fdroidcl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdroidcl">
  <a href="/en/common/fdroidcl.html">fdroidcl</a> <a href="#fdroidcl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F-Droid CLI client.
> More information: <https://github.com/mvdan/fdroidcl>.

#### Fetch the F-Droid index:
```shell
fdroidcl update
```
#### Display info about an app:
```shell
fdroidcl show {{app_id}}
```
#### Download an APK file:
```shell
fdroidcl download {{app_id}}
```
#### Search for an app in the index:
```shell
fdroidcl search {{search_pattern}}
```
#### Install an app on a connected device:
```shell
fdroidcl install {{app_id}}
```
{% endraw %}