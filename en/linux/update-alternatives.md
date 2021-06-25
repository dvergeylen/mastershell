---
layout: default
title: "update-alternatives"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="update-alternatives">
  <a href="/en/linux/update-alternatives.html">update-alternatives</a> <a href="#update-alternatives"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A convenient tool for maintaining symbolic links to determine default commands.

#### Add a symbolic link:
```shell
sudo update-alternatives --install {{path/to/symlink}} {{command_name}} {{path/to/command_binary}} {{priority}}
```
#### Configure a symbolic link for `java`:
```shell
sudo update-alternatives --config {{java}}
```
#### Remove a symbolic link:
```shell
sudo update-alternatives --remove {{java}} {{/opt/java/jdk1.8.0_102/bin/java}}
```
#### Display information about a specified command:
```shell
update-alternatives --display {{java}}
```
#### Display all commands and their current selection:
```shell
update-alternatives --get-selections
```
{% endraw %}