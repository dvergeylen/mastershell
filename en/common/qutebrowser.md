---
layout: default
title: "qutebrowser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qutebrowser">
  <a href="/en/common/qutebrowser.html">qutebrowser</a> <a href="#qutebrowser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A keyboard-driven, vim-like browser based on PyQt5.
> More information: <https://qutebrowser.org/>.

#### Open qutebrowser with a specified storage directory:
```shell
qutebrowser --basedir {{path/to/directory}}
```
#### Open a qutebrowser instance with temporary settings:
```shell
qutebrowser --set {{content.geolocation}} {{true|false}}
```
#### Restore a named session of a qutebrowser instance:
```shell
qutebrowser --restore {{session_name}}
```
#### Launch qutebrowser, opening all URLs using the specified method:
```shell
qutebrowser --target {{auto|tab|tab-bg|tab-silent|tab-bg-silent|window|private-window}}
```
#### Open qutebrowser with a temporary base directory and print logs to stdout as JSON:
```shell
qutebrowser --temp-basedir --json-logging
```
{% endraw %}