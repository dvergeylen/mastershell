---
layout: default
title: "wodim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wodim">
  <a href="/en/linux/wodim.html">wodim</a> <a href="#wodim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command (aliased as `cdrecord` on some systems) for recording data to CDs or DVDs.
> Some invocations of wodim can cause destructive actions, such as erasing all the data on a disc.

#### Display optical drives available to `wodim`:
```shell
wodim --devices
```
#### Record ("burn") an audio-only disc:
```shell
wodim dev=/dev/{{optical_drive}} -audio {{track*.cdaudio}}
```
#### Burn a file to a disc, ejecting the disc once done (some recorders require this):
```shell
wodim -eject dev=/dev/{{optical_drive}} -data {{file.iso}}
```
#### Burn a file to the disc in an optical drive, potentially writing to multiple discs in succession:
```shell
wodim -tao dev=/dev/{{optical_drive}} -data {{file.iso}}
```
{% endraw %}