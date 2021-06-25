---
layout: default
title: "amass viz"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amass-viz">
  <a href="/en/common/amass-viz.html">amass viz</a> <a href="#amass-viz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visualize gathered information in a network graph.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-viz-subcommand>.

#### Generate a D3.js visualization based on database data:
```shell
amass viz -d3 -dir {{path/to/database_directory}}
```
#### Generate a DOT file based on database data:
```shell
amass viz -dot -dir {{path/to/database_directory}}
```
#### Generate a Gephi Graph Exchange XML Format (GEXF) file based on database data:
```shell
amass viz -gexf -dir {{path/to/database_directory}}
```
#### Generate a Graphistry JSON file based on database data:
```shell
amass viz -graphistry -dir {{path/to/database_directory}}
```
#### Generate a Maltego CSV file based on database data:
```shell
amass viz -maltego -dir {{path/to/database_directory}}
```
{% endraw %}