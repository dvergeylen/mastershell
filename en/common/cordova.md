---
layout: default
title: "cordova"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cordova">
  <a href="/en/common/cordova.html">cordova</a> <a href="#cordova"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mobile apps with HTML, CSS & JS.
> More information: <https://cordova.apache.org/docs/en/latest/guide/cli/>.

#### Create a cordova project:
```shell
cordova create {{path}} {{package_name}} {{project_name}}
```
#### Display the current workspace status:
```shell
cordova info
```
#### Add a cordova platform:
```shell
cordova platform add {{platform}}
```
#### Remove a cordova platform:
```shell
cordova platform remove {{platform}}
```
#### Add a cordova plugin:
```shell
cordova plugin add {{pluginid}}
```
#### Remove a cordova plugin:
```shell
cordova plugin remove {{pluginid}}
```
{% endraw %}