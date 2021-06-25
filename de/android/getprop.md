---
layout: default
title: "getprop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getprop">
  <a href="/de/android/getprop.html">getprop</a> <a href="#getprop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Informationen über Android-Systemeigenschaften.
> Weitere Informationen: <https://manned.org/getprop>.

#### Gib Informationen über Android-Systemeigenschaften aus:
```shell
getprop
```
#### Gib Informationen über eine bestimmte Systemeigenschaft aus:
```shell
getprop {{eigenschaft}}
```
#### Gib das SDK-API-Level aus:
```shell
getprop {{ro.build.version.sdk}}
```
#### Gib die Android-Version aus:
```shell
getprop {{ro.build.version.release}}
```
#### Gib das Modell des Geräts aus:
```shell
getprop {{ro.vendor.product.model}}
```
#### Gib den OEM-Entsperrstatus aus:
```shell
getprop {{ro.oem_unlock_supported}}
```
#### Gib die MAC-Adresse der WiFi-Karte aus:
```shell
getprop {{ro.boot.wifimacaddr}}
```
{% endraw %}