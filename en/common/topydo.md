---
layout: default
title: "topydo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="topydo">
  <a href="/en/common/topydo.html">topydo</a> <a href="#topydo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A todo list application that uses the todo.txt format.
> More information: <https://github.com/topydo/topydo>.

#### Add a todo to a specific project with a given context:
```shell
topydo add "{{todo_message}} +{{project_name}} @{{context_name}}"
```
#### Add a todo with a due date of tomorrow with a priority of `A`:
```shell
topydo add "(A) {{todo _message}} due:{{1d}}"
```
#### Add a todo with a due date of friday:
```shell
topydo add "{{todo_message}} due:{{fri}}"
```
#### Add a non-strict repeating todo (next due = now + rec):
```shell
topydo add "water flowers due:{{mon}} rec:{{1w}}"
```
#### Add a strict repeating todo (next due = currentdue + rec):
```shell
topydo add "{{todo_message}} due:{{2020-01-01}} rec:{{+1m}}"
```
#### Revert the last `topydo` command executed:
```shell
topydo revert
```
{% endraw %}