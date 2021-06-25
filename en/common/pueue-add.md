---
layout: default
title: "pueue add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-add">
  <a href="/en/common/pueue-add.html">pueue add</a> <a href="#pueue-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enqueue a task for execution.
> More information: <https://github.com/Nukesor/pueue>.

#### Add any command to the default queue:
```shell
pueue add {{command}}
```
#### Pass a list of flags or arguments to a command when enqueuing:
```shell
pueue add -- {{command --arg -f}}
```
#### Add a command but do not start it if it's the first in a queue:
```shell
pueue add --stashed -- {{rsync --archive --compress /local/directory /remote/directory}}
```
#### Add a command to a group and start it immediately, see `pueue group` to manage groups:
```shell
pueue add --immediate --group "{{CPU_intensive}}" -- {{ffmpeg -i input.mp4 frame_%d.png}}
```
#### Add a command and start it after commands 9 and 12 finish successfully:
```shell
pueue add --after {{9}} {{12}} --group "{{torrents}}" -- {{transmission-cli torrent_file.torrent}}
```
#### Add a command with a label after some delay has passed, see `pueue enqueue` for valid datetime formats:
```shell
pueue add --label "{{compressing large file}}" --delay "{{wednesday 10:30pm}}" -- "{{7z a compressed_file.7z large_file.xml}}"
```
{% endraw %}