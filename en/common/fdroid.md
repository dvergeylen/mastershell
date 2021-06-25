---
layout: default
title: "fdroid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdroid">
  <a href="/en/common/fdroid.html">fdroid</a> <a href="#fdroid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F-Droid build tool.
> F-Droid is an installable catalog of FOSS (Free and Open Source Software) applications for the Android platform.
> More information: <https://f-droid.org/>.

#### Build a specific app:
```shell
fdroid build {{app_id}}
```
#### Build a specific app in a build server VM:
```shell
fdroid build {{app_id}} --server
```
#### Publish the app to the local repository:
```shell
fdroid publish {{app_id}}
```
#### Install the app on every connected device:
```shell
fdroid install {{app_id}}
```
#### Check if the metadata is formatted correctly:
```shell
fdroid lint --format {{app_id}}
```
#### Fix the formatting automatically (if possible):
```shell
fdroid rewritemeta {{app_id}}
```
{% endraw %}