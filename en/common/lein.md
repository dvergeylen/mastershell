---
layout: default
title: "lein"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lein">
  <a href="/en/common/lein.html">lein</a> <a href="#lein"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Clojure projects with declarative configuration.
> More information: <https://leiningen.org>.

#### Generate scaffolding for a new project based on a template:
```shell
lein new {{template_name}} {{project_name}}
```
#### Start a REPL session either with the project or standalone:
```shell
lein repl
```
#### Run the project's `-main` function with optional args:
```shell
lein run {{args}}
```
#### Run the project's tests:
```shell
lein test
```
#### Package up the project files and all its dependencies into a jar file:
```shell
lein uberjar
```
{% endraw %}