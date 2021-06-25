---
layout: default
title: "choco search"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-search">
  <a href="/en/windows/choco-search.html">choco search</a> <a href="#choco-search"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search for a local or remote package with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-search>.

#### Search for a package:
```shell
choco search {{query}}
```
#### Search for a package locally:
```shell
choco search {{query}} --local-only
```
#### Only include exact matches in the results:
```shell
choco search {{query}} --exact
```
#### Confirm all prompts automatically:
```shell
choco search {{query}} --yes
```
#### Specify a custom source to search for packages in:
```shell
choco search {{query}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco search {{query}} --user {{username}} --password {{password}}
```
{% endraw %}