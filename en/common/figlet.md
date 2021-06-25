---
layout: default
title: "figlet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="figlet">
  <a href="/en/common/figlet.html">figlet</a> <a href="#figlet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate ASCII banners from user input.
> More information: <http://www.figlet.org/figlet-man.html>.

#### Generate by directly inputting text:
```shell
figlet {{input_text}}
```
#### Use a custom font file:
```shell
figlet {{input_text}} -f {{font_filename}}
```
#### Pipe command output through figlet:
```shell
{{command}} | figlet
```
#### Show available figlet fonts:
```shell
showfigfonts {{optional_string_to_display}}
```
{% endraw %}