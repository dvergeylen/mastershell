---
layout: default
title: "boot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="boot">
  <a href="/en/common/boot.html">boot</a> <a href="#boot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build tooling for the Clojure programming language.
> More information: <https://github.com/boot-clj/boot>.

#### Start a REPL session either with the project or standalone:
```shell
boot repl
```
#### Build a single `uberjar`:
```shell
boot jar
```
#### Learn about a command:
```shell
boot cljs --help
```
#### Generate scaffolding for a new project based on a template:
```shell
boot --dependencies boot/new new --template {{template_name}} --name {{project_name}}
```
#### Build for development (if using the boot/new template):
```shell
boot dev
```
#### Build for production (if using the boot/new template):
```shell
boot prod
```
{% endraw %}