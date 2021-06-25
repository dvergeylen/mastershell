---
layout: default
title: "bundletool dump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bundletool-dump">
  <a href="/en/common/bundletool-dump.html">bundletool dump</a> <a href="#bundletool-dump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to manipulate Android Application Bundles.
> More information: <https://developer.android.com/studio/command-line/bundletool>.

#### Display the `AndroidManifest.xml` of the base module:
```shell
bundletool dump manifest --bundle={{path/to/bundle.aab}}
```
#### Display a specific value from the `AndroidManifest.xml` using XPath:
```shell
bundletool dump manifest --bundle={{path/to/bundle.aab}} --xpath={{/manifest/@android:versionCode}}
```
#### Display the `AndroidManifest.xml` of a specific module:
```shell
bundletool dump manifest --bundle={{path/to/bundle.aab}} --module={{name}}
```
#### Display all the resources in the application bundle:
```shell
bundletool dump resources --bundle={{path/to/bundle.aab}}
```
#### Display the configuration for a specific resource:
```shell
bundletool dump resources --bundle={{path/to/bundle.aab}} --resource={{type/name}}
```
#### Display the configuration and values for a specific resource using the ID:
```shell
bundletool dump resources --bundle={{path/to/bundle.aab}} --resource={{0x7f0e013a}} --values
```
#### Display the contents of the bundle configuration file:
```shell
bundletool dump config --bundle={{path/to/bundle.aab}}
```
{% endraw %}