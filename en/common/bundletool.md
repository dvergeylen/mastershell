---
layout: default
title: "bundletool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bundletool">
  <a href="/en/common/bundletool.html">bundletool</a> <a href="#bundletool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to manipulate Android Application Bundles.
> More information: <https://developer.android.com/studio/command-line/bundletool>.

#### Display help for a subcommand:
```shell
bundletool help {{subcommand}}
```
#### Generate APKs from an application bundle (prompts for keystore password):
```shell
bundletool build-apks --bundle={{path/to/bundle.aab}} --ks={{path/to/key.keystore}} --ks-key-alias={{key_alias}} --output={{path/to/file.apks}}
```
#### Generate APKs from an application bundle giving the keystore password:
```shell
bundletool build-apks --bundle={{path/to/bundle.aab}} --ks={{path/to/key.keystore}} --ks-key-alias={{key_alias}} –ks-pass={{pass:the_password}} --output={{path/to/file.apks}}
```
#### Generate APKs including only one single APK for universal usage:
```shell
bundletool build-apks --bundle={{path/to/bundle.aab}} --mode={{universal}} --ks={{path/to/key.keystore}} --ks-key-alias={{key_alias}} --output={{path/to/file.apks}}
```
#### Install the right combination of APKs to an emulator or device:
```shell
bundletool install-apks --apks={{path/to/file.apks}}
```
#### Estimate the download size of an application:
```shell
bundletool get-size total --apks={{path/to/file.apks}}
```
#### Generate a device specification JSON file for an emulator or device:
```shell
bundletool get-device-spec --output={{path/to/file.json}}
```
#### Verify a bundle and display detailed information about it:
```shell
bundletool validate --bundle={{path/to/bundle.aab}}
```
{% endraw %}