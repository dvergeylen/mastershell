---
layout: default
title: "choco info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-info">
  <a href="/en/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display detailed information about a package with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-info>.

#### Display information on a specific package:
```shell
choco info {{package}}
```
#### Display information for a local package only:
```shell
choco info {{package}} --local-only
```
#### Specify a custom source to receive packages information from:
```shell
choco info {{package}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco info {{package}} --user {{username}} --password {{password}}
```
{% endraw %}