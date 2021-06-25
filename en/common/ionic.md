---
layout: default
title: "ionic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ionic">
  <a href="/en/common/ionic.html">ionic</a> <a href="#ionic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A framework to build hybrid mobile apps.
> More information: <https://ionicframework.com/docs/cli>.

#### Create a new project:
```shell
ionic start
```
#### Start a local dev server for app dev/testing:
```shell
ionic serve
```
#### Generate new app component, directive, page, pipe, provider or tabs:
```shell
ionic g {{page}}
```
#### Show versions of ionic, cordova, environment, etc.:
```shell
ionic info
```
#### Run app on an android/ios device:
```shell
ionic cordova run {{android|ios}} --device
```
#### Check the health of a ionic app:
```shell
ionic doctor {{check}}
```
{% endraw %}