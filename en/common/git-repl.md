---
layout: default
title: "git repl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-repl">
  <a href="/en/common/git-repl.html">git repl</a> <a href="#git-repl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git REPL (read-evaluate-print-loop) - an interactive Git shell.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-repl>.

#### Start an interactive Git shell:
```shell
git repl
```
#### Run a Git command while in the interactive Git shell:
```shell
{{git_subcommand}} {{command_arguments}}
```
#### Run an external (non-Git) command while in the interactive Git shell:
```shell
!{{command}} {{command_arguments}}
```
#### Exit the interactive Git shell (or press Ctrl + D):
```shell
exit
```
{% endraw %}