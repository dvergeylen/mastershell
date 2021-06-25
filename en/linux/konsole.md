---
layout: default
title: "konsole"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="konsole">
  <a href="/en/linux/konsole.html">konsole</a> <a href="#konsole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konsole: The KDE terminal emulator.
> More information: <https://konsole.kde.org>.

#### Open a new Konsole in a specific directory:
```shell
konsole --workdir {{path/to/directory}}
```
#### Run a specific command and do not close the window after it exits:
```shell
konsole --noclose -e {{command}}
```
#### Open a new tab:
```shell
konsole --new-tab
```
#### Open a Konsole in the background and bring to the front when Ctrl+Shift+F12 (by default) is pressed:
```shell
konsole --background-mode
```
#### Open a Konsole with the emergency FALLBACK profile:
```shell
konsole --fallback-profile
```
{% endraw %}