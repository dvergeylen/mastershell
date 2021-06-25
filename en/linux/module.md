---
layout: default
title: "module"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="module">
  <a href="/en/linux/module.html">module</a> <a href="#module"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modify a users' environment using the module command.
> More information: <https://lmod.readthedocs.io/en/latest/010_user.html>.

#### Display available modules:
```shell
module avail
```
#### Search for a module by name:
```shell
module spider {{module_name}}
```
#### Load a module:
```shell
module load {{module_name}}
```
#### Display loaded modules:
```shell
module list
```
#### Unload a specific loaded module:
```shell
module {{module_name}}
```
#### Unload all loaded modules:
```shell
module purge
```
{% endraw %}