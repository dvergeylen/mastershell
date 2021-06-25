---
layout: default
title: "nudoku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nudoku">
  <a href="/en/common/nudoku.html">nudoku</a> <a href="#nudoku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sudoku game in terminal.
> More information: <https://jubalh.github.io/nudoku/>.

#### Start a sudoku game:
```shell
nudoku
```
#### Choose the difficulty of the game:
```shell
nudoku -d {{easy|normal|hard}}
```
#### Navigate the board:
```shell
{{h|j|k|l}} OR {{Left|Down|Up|Right}} arrow key
```
#### Delete a number:
```shell
{{Backspace|x}}
```
#### Get a hint:
```shell
H
```
#### See the complete solution:
```shell
S
```
#### Create a new puzzle:
```shell
N
```
#### Quit the game:
```shell
Q
```
{% endraw %}