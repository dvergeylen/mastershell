---
layout: default
title: "choco upgrade"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-upgrade">
  <a href="/en/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Upgrade one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-upgrade>.

#### Upgrade one or more space-separated packages:
```shell
choco upgrade {{package(s)}}
```
#### Upgrade to a specific version of a package:
```shell
choco upgrade {{package}} --version {{version}}
```
#### Upgrade all packages:
```shell
choco upgrade all
```
#### Upgrade all except specified comma-separated packages:
```shell
choco upgrade all --except "{{package(s)}}"
```
#### Confirm all prompts automatically:
```shell
choco upgrade {{package}} --yes
```
#### Specify a custom source to receive packages from:
```shell
choco upgrade {{package}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco upgrade {{package}} --user {{username}} --password {{password}}
```
{% endraw %}