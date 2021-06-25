---
layout: default
title: "pulseaudio"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pulseaudio">
  <a href="/en/linux/pulseaudio.html">pulseaudio</a> <a href="#pulseaudio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The pulseaudio sound system daemon and manager.
> More information: <https://www.freedesktop.org/wiki/Software/PulseAudio/>.

#### Check if pulseaudio is running (a non-zero exit code means it is not running):
```shell
pulseaudio --check
```
#### Start the pulseaudio daemon in the background:
```shell
pulseaudio --start
```
#### Kill the running pulseaudio daemon:
```shell
pulseaudio --kill
```
#### List available modules:
```shell
pulseaudio --dump-modules
```
#### Load a module into the currently running daemon with the specified arguments:
```shell
pulseaudio --load="{{module_name}} {{arguments}}"
```
{% endraw %}