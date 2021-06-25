---
layout: default
title: "arch-chroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arch-chroot">
  <a href="/en/linux/arch-chroot.html">arch-chroot</a> <a href="#arch-chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enhanced `chroot` command to help in the Arch Linux installation process.
> More information: <https://man.archlinux.org/man/arch-chroot.8>.

#### Start an interactive shell (`bash`, by default) in a new root directory:
```shell
arch-chroot {{path/to/new/root}}
```
#### Specify the user (other than the current user) to run the shell as:
```shell
arch-chroot -u {{user}} {{path/to/new/root}}
```
#### Run a custom command (instead of the default `bash`) in the new root directory:
```shell
arch-chroot {{path/to/new/root}} {{command}} {{command_arguments}}
```
#### Specify the shell, other than the default `bash` (in this case, the `zsh` package should have been installed in the target system):
```shell
arch-chroot {{path/to/new/root}} {{zsh}}
```
{% endraw %}