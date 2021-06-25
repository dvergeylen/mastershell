---
layout: default
title: "iwctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iwctl">
  <a href="/en/linux/iwctl.html">iwctl</a> <a href="#iwctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for controlling the iwd network supplicant.
> More information: <https://iwd.wiki.kernel.org/gettingstarted>.

#### Start the interactive mode, in this mode you can enter the commands directly, with autocompletion:
```shell
iwctl
```
#### Call general help:
```shell
iwctl --help
```
#### Display your wifi stations:
```shell
iwctl station list
```
#### Start looking for networks with a station:
```shell
iwctl station {{station}} scan
```
#### Display the networks found by a station:
```shell
iwctl station {{station}} get-networks
```
#### Connect to a network with a station, if credentials are needed they will be asked:
```shell
iwctl station {{station}} connect {{network_name}}
```
{% endraw %}