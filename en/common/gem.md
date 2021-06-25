---
layout: default
title: "gem"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gem">
  <a href="/en/common/gem.html">gem</a> <a href="#gem"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with the package manager for the Ruby programming language.
> More information: <https://rubygems.org>.

#### Search for remote gem(s) and show all available versions:
```shell
gem search {{regular_expression}} --all
```
#### Install latest version of a gem:
```shell
gem install {{gemname}}
```
#### Install specific version of a gem:
```shell
gem install {{gemname}} --version {{1.0.0}}
```
#### Install the latest matching (SemVer) version of a gem:
```shell
gem install {{gemname}} --version '~> {{1.0}}'
```
#### Update a gem:
```shell
gem update {{gemname}}
```
#### List all local gems:
```shell
gem list
```
#### Uninstall a gem:
```shell
gem uninstall {{gemname}}
```
#### Uninstall specific version of a gem:
```shell
gem uninstall {{gemname}} --version {{1.0.0}}
```
{% endraw %}