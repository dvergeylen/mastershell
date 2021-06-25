---
layout: default
title: "choco outdated"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-outdated">
  <a href="/en/windows/choco-outdated.html">choco outdated</a> <a href="#choco-outdated"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check for outdated packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-outdated>.

#### Display a list of outdated packages in table format:
```shell
choco outdated
```
#### Ignore pinned packages in the output:
```shell
choco outdated --ignore-pinned
```
#### Specify a custom source to check packages from:
```shell
choco outdated --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco outdated --user {{username}} --password {{password}}
```
{% endraw %}