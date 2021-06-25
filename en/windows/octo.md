---
layout: default
title: "octo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="octo">
  <a href="/en/windows/octo.html">octo</a> <a href="#octo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tools for Octopus Deploy.
> More information: <https://octopus.com/docs/octopus-rest-api/octo.exe-command-line>.

#### Create a package:
```shell
octo pack --id={{package_name}}
```
#### Push a package to a repository on the Octopus server:
```shell
octo push --package={{package_name}}
```
#### Create a release:
```shell
octo create-release --project={{project_name}} --packageversion={{version}}
```
#### Deploy a release:
```shell
octo deploy-release --project={{project_name}} --packageversion={{version}} --deployto={{environment_name}} --tenant={{deployment_target}}
```
{% endraw %}