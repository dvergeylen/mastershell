---
layout: default
title: "bootctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bootctl">
  <a href="/en/common/bootctl.html">bootctl</a> <a href="#bootctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control EFI firmware boot settings and manage boot loader.
> More information: <https://man.archlinux.org/man/bootctl.1>.

#### Show information about the system firmware and the bootloaders:
```shell
sudo bootctl status
```
#### Set a flag to boot into the system firmware on the next boot (similar to `sudo systemctl reboot --firmware-setup`):
```shell
sudo bootctl reboot-to-firmware true
```
#### Specify the path to the EFI system partition (defaults to `/efi/`, `/boot/` or `/boot/efi`):
```shell
sudo bootctl --esp-path={{/path/to/efi_system_partition/}}
```
#### Show all available bootloader entries:
```shell
sudo bootctl list
```
#### Install `systemd-boot` into the EFI system partition:
```shell
sudo bootctl install
```
#### Remove all installed versions of `systemd-boot` from the EFI system partition:
```shell
sudo bootctl remove
```
{% endraw %}