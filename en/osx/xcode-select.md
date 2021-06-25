---
layout: default
title: "xcode-select"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcode-select">
  <a href="/en/osx/xcode-select.html">xcode-select</a> <a href="#xcode-select"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch between different versions of Xcode and the included developer tools.
> Also used to update the path to Xcode if it is moved after installation.

#### Install Xcode's command-line tools:
```shell
xcode-select --install
```
#### Select a given path as the active developer directory:
```shell
xcode-select -s {{path/to/Xcode.app/Contents/Developer}}
```
#### Select a given Xcode instance and use its developer directory as the active one:
```shell
xcode-select -s {{path/to/Xcode.app}}
```
#### Print the currently selected developer directory:
```shell
xcode-select -p
```
#### Discard any user-specified developer directory so that it will be found via the default search mechanism:
```shell
sudo xcode-select -r
```
{% endraw %}