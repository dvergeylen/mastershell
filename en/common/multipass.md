---
layout: default
title: "multipass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="multipass">
  <a href="/en/common/multipass.html">multipass</a> <a href="#multipass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI to manage Ubuntu virtual machines using native hypervisors.
> More information: <https://multipass.run/>.

#### List the aliases that can be used to launch an instance:
```shell
multipass find
```
#### Launch a new instance, set its name and use a cloud-init configuration file:
```shell
multipass launch -n {{instance_name}} --cloud-init {{configuration_file}}
```
#### List all the created instances and some of their properties:
```shell
multipass list
```
#### Start a specific instance by name:
```shell
multipass start {{instance_name}}
```
#### Show the properties of an instance:
```shell
multipass info {{instance_name}}
```
#### Open a shell prompt on a specific instance by name:
```shell
multipass shell {{instance_name}}
```
#### Delete an instance by name:
```shell
multipass delete {{instance_name}}
```
#### Mount a directory into a specific instance:
```shell
multipass mount {{path/to/local/directory}} {{instance_name}}:{{path/to/target/directory}}
```
{% endraw %}