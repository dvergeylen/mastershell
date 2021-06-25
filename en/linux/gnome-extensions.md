---
layout: default
title: "gnome-extensions"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gnome-extensions">
  <a href="/en/linux/gnome-extensions.html">gnome-extensions</a> <a href="#gnome-extensions"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage gnome extensions from the terminal.
> More information: <https://wiki.gnome.org/Projects/GnomeShell/Extensions>.

#### Display the version:
```shell
gnome-extensions version
```
#### List all the installed extensions:
```shell
gnome-extensions list
```
#### Display information about a specific extension:
```shell
gnome-extensions info "{{extension_id}}"
```
#### Display help for a subcommand (like `list`):
```shell
gnome-extensions help {{subcommand}}
```
#### Enable a specific extension:
```shell
gnome-extensions enable "{{extension_id}}"
```
#### Disable a specific extension:
```shell
gnome-extension disable "{{extension_id}}"
```
#### Uninstall a specific extension:
```shell
gnome-extension uninstall "{{extension_id}}"
```
{% endraw %}