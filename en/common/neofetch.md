---
layout: default
title: "neofetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="neofetch">
  <a href="/en/common/neofetch.html">neofetch</a> <a href="#neofetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI tool to display information about your operating system, software and hardware.
> More information: <https://github.com/dylanaraps/neofetch>.

#### Return the default config, and create it if it's the first time the program runs:
```shell
neofetch
```
#### Trigger an info line from appearing in the output, where 'infoname' is the function name in the config file, e.g. memory:
```shell
neofetch --{{enable|disable}} {{infoname}}
```
#### Hide/Show OS architecture:
```shell
neofetch --os_arch {{on|off}}
```
#### Enable/Disable CPU brand in output:
```shell
neofetch --cpu_brand {{on|off}}
```
{% endraw %}