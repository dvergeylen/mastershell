---
layout: default
title: "asr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asr">
  <a href="/en/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restore (copy) a disk image onto a volume.
> The command name stands for Apple Software Restore.

#### Restore a disk image to a target volume:
```shell
sudo asr restore --source {{image_name}}.dmg --target {{path/to/volume}}
```
#### Erase the target volume before restoring:
```shell
sudo asr restore --source {{image_name}}.dmg --target {{path/to/volume}} --erase
```
#### Skip verification after restoring:
```shell
sudo asr restore --source {{image_name}}.dmg --target {{path/to/volume}} --noverify
```
#### Clone volumes without the use of an intermediate disk image:
```shell
sudo asr restore --source {{path/to/volume}} --target {{path/to/cloned_volume}}
```
{% endraw %}