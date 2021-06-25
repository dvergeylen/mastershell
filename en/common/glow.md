---
layout: default
title: "glow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="glow">
  <a href="/en/common/glow.html">glow</a> <a href="#glow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Render Markdown in the terminal.
> More information: <https://github.com/charmbracelet/glow>.

#### Run glow and select a file to view:
```shell
glow
```
#### Render a Markdown file to the terminal:
```shell
glow {{path/to/file}}
```
#### View a Markdown file using a paginator:
```shell
glow -p {{path/to/file}}
```
#### View a file from a URL:
```shell
glow {{https://example.com/file.md}}
```
#### View a GitHub/GitLab README:
```shell
glow {{github.com/owner/repository}}
```
{% endraw %}