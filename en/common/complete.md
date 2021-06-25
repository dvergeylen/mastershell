---
layout: default
title: "complete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="complete">
  <a href="/en/common/complete.html">complete</a> <a href="#complete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provides argument autocompletion to shell commands.
> More information: <https://www.gnu.org/software/bash/manual/html_node/Programmable-Completion-Builtins.html>.

#### Apply a function that performs autocompletion to a command:
```shell
complete -F {{function}} {{command}}
```
#### Apply a command that performs autocompletion to another command:
```shell
complete -C {{autocomplete_command}} {{command}}
```
#### Apply autocompletion without appending a space to the completed word:
```shell
complete -o nospace -F {{function}} {{command}}
```
{% endraw %}