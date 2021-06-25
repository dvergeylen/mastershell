---
layout: default
title: "stty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stty">
  <a href="/en/common/stty.html">stty</a> <a href="#stty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set options for a terminal device interface.
> More information: <https://www.gnu.org/software/coreutils/stty>.

#### Display all settings for the current terminal:
```shell
stty -a
```
#### Set the number of rows:
```shell
stty rows {{rows}}
```
#### Set the number of columns:
```shell
stty cols {{cols}}
```
#### Get the actual transfer speed of a device:
```shell
stty -F {{path/to/device_file}} speed
```
#### Reset all modes to reasonable values for the current terminal:
```shell
stty sane
```
{% endraw %}