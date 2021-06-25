---
layout: default
title: "git mergetool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mergetool">
  <a href="/en/common/git-mergetool.html">git mergetool</a> <a href="#git-mergetool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run merge conflict resolution tools to resolve merge conflicts.
> More information: <https://git-scm.com/docs/git-mergetool>.

#### Launch the default merge tool to resolve conflicts:
```shell
git mergetool
```
#### List valid merge tools:
```shell
git mergetool --tool-help
```
#### Launch the merge tool identified by a name:
```shell
git mergetool --tool {{tool_name}}
```
#### Don't prompt before each invocation of the merge tool:
```shell
git mergetool --no-prompt
```
#### Explicitly use the GUI merge tool (see the `merge.guitool` config variable):
```shell
git mergetool --gui
```
#### Explicitly use the regular merge tool (see the `merge.tool` config variable):
```shell
git mergetool --no-gui
```
{% endraw %}