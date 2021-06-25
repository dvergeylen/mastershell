---
layout: default
title: "dolphin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dolphin">
  <a href="/en/linux/dolphin.html">dolphin</a> <a href="#dolphin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE file manager.
> More information: <https://apps.kde.org/dolphin/>.

#### Launch Dolphin:
```shell
dolphin
```
#### Launch Dolphin and display a specific directory:
```shell
dolphin {{path/to/directory}}
```
#### Launch Dolphin with a specific file or directory selected:
```shell
dolphin --select {{path/to/file_or_directory}}
```
#### Launch Dolphin in a separated window:
```shell
dolphin --new-window
```
#### Launch Dolphin in split view:
```shell
dolphin --split
```
#### Start the Dolphin daemon (only required to use the DBus interface):
```shell
dolphin --daemon
```
#### Display help:
```shell
dolphin --help
```
{% endraw %}