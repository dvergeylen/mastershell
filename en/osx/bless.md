---
layout: default
title: "bless"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bless">
  <a href="/en/osx/bless.html">bless</a> <a href="#bless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set volume boot capability and startup disk options.
> More information: <https://ss64.com/osx/bless.html>.

#### Bless a volume with only Mac OS X or Darwin, and create the BootX and `boot.efi` files as needed:
```shell
bless --folder "{{/Volumes/Mac OS X/System/Library/CoreServices}}" --bootinfo --bootefi
```
#### Set a volume containing either Mac OS 9 and Mac OS X to be the active volume:
```shell
bless --mount "{{/Volumes/Mac OS}}" --setBoot
```
#### Set the system to NetBoot and broadcast for an available server:
```shell
bless --netboot --server {{bsdp://255.255.255.255}}
```
#### Gather information about the currently selected volume (as determined by the firmware), suitable for piping to a program capable of parsing Property Lists:
```shell
bless --info --plist
```
{% endraw %}