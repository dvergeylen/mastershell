---
layout: default
title: "choco list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-list">
  <a href="/en/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a list of packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-list>.

#### Display all available packages:
```shell
choco list
```
#### Display all locally installed packages:
```shell
choco list --local-only
```
#### Display a list including local programs:
```shell
choco list --include-programs
```
#### Display only approved packages:
```shell
choco list --approved-only
```
#### Specify a custom source to display packages from:
```shell
choco list --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco list --user {{username}} --password {{password}}
```
{% endraw %}