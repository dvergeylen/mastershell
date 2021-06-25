---
layout: default
title: "emacsclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emacsclient">
  <a href="/en/common/emacsclient.html">emacsclient</a> <a href="#emacsclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open files in an existing Emacs server.
> See also `emacs`.
> More information: <https://www.emacswiki.org/emacs/EmacsClient>.

#### Open a file in an existing Emacs server (using GUI if available):
```shell
emacsclient {{path/to/file}}
```
#### Open a file in console mode (without an X window):
```shell
emacsclient --no-window-system {{path/to/file}}
```
#### Open a file in a new Emacs window:
```shell
emacsclient --create-frame {{path/to/file}}
```
#### Evaluate a command, printing the output to stdout, and then quit:
```shell
emacsclient --eval '({{command}})'
```
#### Specify an alternative editor in case no Emacs server is running:
```shell
emacsclient --alternate-editor {{editor}} {{path/to/file}}
```
#### Stop a running Emacs server and all its instances, asking for confirmation on unsaved files:
```shell
emacsclient --eval '(save-buffers-kill-emacs)'
```
{% endraw %}