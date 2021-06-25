---
layout: default
title: "tb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tb">
  <a href="/en/common/tb.html">tb</a> <a href="#tb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for managing tasks and notes across multiple boards.
> More information: <https://github.com/klaussinani/taskbook>.

#### Add a new task to a board:
```shell
tb --task {{task_description}} @{{board_name}}
```
#### Add a new note to a board:
```shell
tb --note {{note_description}} @{{board_name}}
```
#### Edit item's priority:
```shell
tb --priority @{{item_id}} {{priority}}
```
#### Check/uncheck item:
```shell
tb --check {{item_id}}
```
#### Archive all checked items:
```shell
tb --clear
```
#### Move item to a board:
```shell
tb --move @{{item_id}} {{board_name}}
```
{% endraw %}