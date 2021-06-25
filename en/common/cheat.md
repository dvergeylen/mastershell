---
layout: default
title: "cheat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cheat">
  <a href="/en/common/cheat.html">cheat</a> <a href="#cheat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and view interactive cheat sheets on the command-line.
> More information: <https://github.com/cheat/cheat>.

#### Show example usage of a command:
```shell
cheat {{command}}
```
#### Edit the cheat sheet for a command:
```shell
cheat -e {{command}}
```
#### List the available cheat sheets:
```shell
cheat -l
```
#### Search available the cheat sheets for a specified command name:
```shell
cheat -s {{command}}
```
#### Get the current cheat version:
```shell
cheat -v
```
{% endraw %}