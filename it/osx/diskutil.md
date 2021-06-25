---
layout: default
title: "diskutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diskutil">
  <a href="/it/osx/diskutil.html">diskutil</a> <a href="#diskutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per gestire i dischi locali e i volumi.

#### Mostra tutti i dischi correnti, le partizioni e i volumi montati:
```shell
diskutil list
```
#### Ripara le strutture dati del filesystem di un volume:
```shell
diskutil repairVolume {{/dev/diskX}}
```
#### Smonta un volume:
```shell
diskutil unmountDisk {{/dev/diskX}}
```
#### Estrai un CD/DVD (smontando prima dell'estrazione):
```shell
diskutil eject {{/dev/disk1}}
```
{% endraw %}