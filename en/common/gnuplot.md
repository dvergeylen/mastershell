---
layout: default
title: "gnuplot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gnuplot">
  <a href="/en/common/gnuplot.html">gnuplot</a> <a href="#gnuplot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A graph plotter that outputs in several formats.
> More information: <http://www.gnuplot.info/>.

#### Start the interactive graph plotting shell:
```shell
gnuplot
```
#### Plot the graph for the specified graph definition file:
```shell
gnuplot {{path/to/definition.plt}}
```
#### Set the output format by executing a command before loading the definition file:
```shell
gnuplot -e "{{set output "path/to/filename.png" size 1024,768}}" {{path/to/definition.plt}}
```
#### Persist the graph plot preview window after gnuplot exits:
```shell
gnuplot --persist {{path/to/definition.plt}}
```
{% endraw %}