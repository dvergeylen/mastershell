---
layout: default
title: "choco install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-install">
  <a href="/en/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-install>.

#### Install one or more space-separated packages:
```shell
choco install {{package(s)}}
```
#### Install packages from a custom configuration file:
```shell
choco install {{path/to/packages.config}}
```
#### Install a specific nuspec or nupkg file:
```shell
choco install {{path/to/file}}
```
#### Install a specific version of a package:
```shell
choco install {{package}} --version {{version}}
```
#### Allow installing multiple versions of a package:
```shell
choco install {{package}} --allow-multiple
```
#### Confirm all prompts automatically:
```shell
choco install {{package}} --yes
```
#### Specify a custom source to receive packages from:
```shell
choco install {{package}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco install {{package}} --user {{username}} --password {{password}}
```
{% endraw %}