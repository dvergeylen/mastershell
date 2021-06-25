---
layout: default
title: "jrnl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jrnl">
  <a href="/en/common/jrnl.html">jrnl</a> <a href="#jrnl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple journal application for your command-line.
> More information: <http://jrnl.sh>.

#### Insert a new entry with your editor:
```shell
jrnl
```
#### Quickly insert a new entry:
```shell
jrnl {{today at 3am}}: {{title}}. {{content}}
```
#### View the last ten entries:
```shell
jrnl -n {{10}}
```
#### View everything that happened from the start of last year to the start of last march:
```shell
jrnl -from "{{last year}}" -until {{march}}
```
#### Edit all entries tagged with "texas" and "history":
```shell
jrnl {{@texas}} -and {{@history}} --edit
```
{% endraw %}