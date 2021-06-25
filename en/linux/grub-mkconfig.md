---
layout: default
title: "grub-mkconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grub-mkconfig">
  <a href="/en/linux/grub-mkconfig.html">grub-mkconfig</a> <a href="#grub-mkconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a GRUB configuration file.
> More information: <https://www.gnu.org/software/grub/manual/grub/html_node/Invoking-grub_002dmkconfig.html>.

#### Do a dry run and print the configuration to stdout:
```shell
sudo grub-mkconfig
```
#### Generate the configuration file:
```shell
sudo grub-mkconfig --output={{/boot/grub/grub.cfg}}
```
#### Print the help page:
```shell
grub-mkconfig --help
```
{% endraw %}