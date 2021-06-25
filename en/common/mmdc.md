---
layout: default
title: "mmdc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mmdc">
  <a href="/en/common/mmdc.html">mmdc</a> <a href="#mmdc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for mermaid, a diagram generation tool with a domain-specific language.
> A mermaid definition file is taken as input and a SVG, PNG, or PDF file is generated as output.
> More information: <https://mermaid-js.github.io/mermaid/>.

#### Convert a file to the specified format (automatically determined from the file extension):
```shell
mmdc --input {{input.mmd}} --output {{output.svg}}
```
#### Specify the theme of the chart:
```shell
mmdc --input {{input.mmd}} --output {{output.svg}} --theme {{forest|dark|neutral|default}}
```
#### Specify the background color of the chart (e.g. `lime`, `"#D8064F"`, or `transparent`):
```shell
mmdc --input {{input.mmd}} --output {{output.svg}} --backgroundColor {{color}}
```
{% endraw %}