---
layout: default
title: "mdp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdp">
  <a href="/en/common/mdp.html">mdp</a> <a href="#mdp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line based tool to make presentations from Markdown files.
> More information: <https://github.com/visit1985/mdp>.

#### Launch a presentation in the terminal from a Markdown file:
```shell
mdp {{presentation.md}}
```
#### Disable fading transitions:
```shell
mdp --nofade {{presentation.md}}
```
#### Invert font colors to use in terminals with light background:
```shell
mdp --invert {{presentation.md}}
```
#### Disable transparency in transparent terminals:
```shell
mdp --notrans {{presentation.md}}
```
{% endraw %}