---
layout: default
title: "pamixer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pamixer">
  <a href="/en/common/pamixer.html">pamixer</a> <a href="#pamixer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple command-line mixer for PulseAudio.
> More information: <https://github.com/cdemoulins/pamixer>.

#### List all sinks and sources with their corresponding IDs:
```shell
pamixer --list-sinks --list-sources
```
#### Set the volume to 75% on the default sink:
```shell
pamixer --set-volume {{75}}
```
#### Toggle mute on a sink other than the default:
```shell
pamixer --toggle-mute --sink {{ID}}
```
#### Increase the volume on default sink by 5%:
```shell
pamixer --increase {{5}}
```
#### Decrease the volume on a source by 5%:
```shell
pamixer --decrease {{5}} --source {{ID}}
```
#### Use the allow boost option to increase, decrease, or set the volume above 100%:
```shell
pamixer --set-volume {{105}} --allow-boost
```
#### Mute the default sink (use `--unmute` instead to unmute):
```shell
pamixer --mute
```
{% endraw %}