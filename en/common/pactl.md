---
layout: default
title: "pactl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pactl">
  <a href="/en/common/pactl.html">pactl</a> <a href="#pactl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control a running PulseAudio sound server.

#### List all sinks (or other types - sinks are outputs and sink-inputs are active audio streams):
```shell
pactl list {{sinks}} short
```
#### Change the default sink (output) to 1 (the number can be retrieved via the `list` subcommand):
```shell
pactl set-default-sink {{1}}
```
#### Move sink-input 627 to sink 1:
```shell
pactl move-sink-input {{627}} {{1}}
```
#### Set the volume of sink 1 to 75%:
```shell
pactl set-sink-volume {{1}} {{0.75}}
```
#### Toggle mute on the default sink (using the special name `@DEFAULT_SINK@`):
```shell
pactl set-sink-mute {{@DEFAULT_SINK@}} toggle
```
{% endraw %}