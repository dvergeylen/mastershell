---
layout: default
title: "history"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="history">
  <a href="/en/common/history.html">history</a> <a href="#history"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line history.
> More information: <https://www.gnu.org/software/bash/manual/html_node/Bash-History-Builtins.html>.

#### Display the commands history list with line numbers:
```shell
history
```
#### Display the last 20 commands:
```shell
history {{20}}
```
#### Clear the commands history list (only for current `bash` shell):
```shell
history -c
```
#### Overwrite history file with history of current `bash` shell (often combined with `history -c` to purge history):
```shell
history -w
```
#### Delete the history entry at the specified offset:
```shell
history -d {{offset}}
```
{% endraw %}