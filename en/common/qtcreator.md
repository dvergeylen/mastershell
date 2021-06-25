---
layout: default
title: "qtcreator"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qtcreator">
  <a href="/en/common/qtcreator.html">qtcreator</a> <a href="#qtcreator"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross-platform IDE for Qt applications.
> More information: <https://doc.qt.io/qtcreator/creator-cli.html>.

#### Start Qt Creator:
```shell
qtcreator
```
#### Start Qt Creator and restore the last session:
```shell
qtcreator -lastsession
```
#### Start Qt Creator but don't load the specified plugin:
```shell
qtcreator -noload {{plugin}}
```
#### Start Qt Creator but don't load any plugins:
```shell
qtcreator -noload {{all}}
```
#### Start Qt Creator in presentation mode with pop-ups for keyboard shortcuts:
```shell
qtcreator -presentationMode
```
#### Start Qt Creator and show the diff from a specific commit:
```shell
qtcreator -git-show {{commit}}
```
{% endraw %}