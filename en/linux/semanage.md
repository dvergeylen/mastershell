---
layout: default
title: "semanage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="semanage">
  <a href="/en/linux/semanage.html">semanage</a> <a href="#semanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SELinux Policy Management tool.
> More information: <https://manned.org/semanage>.

#### Output local customizations:
```shell
semanage -S {{store}} -o {{path/to/output_file}}
```
#### Take a set of commands from a specified file and load them in a single transaction:
```shell
semanage -S {{store}} -i {{path/to/input_file}}
```
#### Manage booleans. Booleans allow the administrator to modify the confinement of processes based on the current configuration:
```shell
semanage boolean -S {{store}} {{--delete|--modify|--list|--noheading|--deleteall}} {{-on|-off}} -F {{boolean|boolean_file}}
```
#### Manage policy modules:
```shell
semanage module -S {{store}} {{--add|--delete|--list|--modify}} {{--enable|--disable}} {{module_name}}
```
#### Disable/Enable dontaudit rules in policy:
```shell
semanage dontaudit -S {{store}} {{on|off}}
```
{% endraw %}