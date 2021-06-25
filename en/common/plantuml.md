---
layout: default
title: "plantuml"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="plantuml">
  <a href="/en/common/plantuml.html">plantuml</a> <a href="#plantuml"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create UML diagrams from a plain text language and render them in different formats.
> More information: <https://plantuml.com/en/command-line>.

#### Render diagrams to default format (PNG):
```shell
plantuml {{diagram1.puml}} {{diagram2.puml}}
```
#### Render a diagram in given format (e.g. `png`, `pdf`, `svg`, `txt`):
```shell
plantuml -t {{format}} {{diagram.puml}}
```
#### Render all diagrams of a directory:
```shell
plantuml {{path/to/diagrams}}
```
#### Render a diagram to the output directory:
```shell
plantuml -o {{path/to/output}} {{diagram.puml}}
```
#### Render a diagram with the configuration file:
```shell
plantuml -config {{config.cfg}} {{diagram.puml}}
```
#### Display help:
```shell
plantuml -help
```
{% endraw %}