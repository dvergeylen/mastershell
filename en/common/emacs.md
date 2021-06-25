---
layout: default
title: "emacs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emacs">
  <a href="/en/common/emacs.html">emacs</a> <a href="#emacs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The extensible, customizable, self-documenting, real-time display editor.
> See also `emacsclient`.
> More information: <https://www.gnu.org/software/emacs>.

#### Start Emacs and open a file:
```shell
emacs {{path/to/file}}
```
#### Open a file at a specified line number:
```shell
emacs +{{line_number}} {{path/to/file}}
```
#### Start Emacs in console mode (without an X window):
```shell
emacs --no-window-system
```
#### Start an Emacs server in the background (accessible via `emacsclient`):
```shell
emacs --daemon
```
#### Stop a running Emacs server and all its instances, asking for confirmation on unsaved files:
```shell
emacsclient --eval '(save-buffers-kill-emacs)'
```
#### Save a file in Emacs:
```shell
Ctrl + X, Ctrl + S
```
#### Quit Emacs:
```shell
Ctrl + X, Ctrl + C
```
{% endraw %}