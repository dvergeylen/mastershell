---
layout: default
title: "sdkmanager"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sdkmanager">
  <a href="/en/common/sdkmanager.html">sdkmanager</a> <a href="#sdkmanager"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to install packages for the Android SDK.
> More information: <https://developer.android.com/studio/command-line/sdkmanager>.

#### List available packages:
```shell
sdkmanager --list
```
#### Install a package:
```shell
sdkmanager {{package}}
```
#### Update every installed package:
```shell
sdkmanager --update
```
#### Uninstall a package:
```shell
sdkmanager --uninstall {{package}}
```
{% endraw %}