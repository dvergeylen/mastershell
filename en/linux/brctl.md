---
layout: default
title: "brctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brctl">
  <a href="/en/linux/brctl.html">brctl</a> <a href="#brctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ethernet bridge administration.

#### Show a list with information about currently existing ethernet bridges:
```shell
sudo brctl show
```
#### Create a new ethernet bridge interface:
```shell
sudo brctl add {{bridge_name}}
```
#### Delete an existing ethernet bridge interface:
```shell
sudo brctl del {{bridge_name}}
```
#### Add an interface to an existing bridge:
```shell
sudo brctl addif {{bridge_name}} {{interface_name}}
```
#### Remove an interface from an existing bridge:
```shell
sudo brctl delif {{bridge_name}} {{interface_name}}
```
{% endraw %}