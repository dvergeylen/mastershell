---
layout: default
title: "fondue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fondue">
  <a href="/en/windows/fondue.html">fondue</a> <a href="#fondue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line installer for optional Windows features.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/fondue>.

#### Enable a specific Windows feature:
```shell
fondue /enable-feature:{{feature}}
```
#### Hide all output messages to the user:
```shell
fondue /enable-feature:{{feature}} /hide-ux:all
```
#### Specify a caller process name for error reporting:
```shell
fondue /enable-feature:{{feature}} /caller-name:{{name}}
```
{% endraw %}