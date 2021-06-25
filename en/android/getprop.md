---
layout: default
title: "getprop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getprop">
  <a href="/en/android/getprop.html">getprop</a> <a href="#getprop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about Android system properties.
> More information: <https://manned.org/getprop>.

#### Display information about Android system properties:
```shell
getprop
```
#### Display information about a specific property:
```shell
getprop {{prop}}
```
#### Display the SDK API level:
```shell
getprop {{ro.build.version.sdk}}
```
#### Display the Android version:
```shell
getprop {{ro.build.version.release}}
```
#### Display the Android device model:
```shell
getprop {{ro.vendor.product.model}}
```
#### Display the OEM unlock status:
```shell
getprop {{ro.oem_unlock_supported}}
```
#### Display the MAC address of the Android's WiFi card:
```shell
getprop {{ro.boot.wifimacaddr}}
```
{% endraw %}