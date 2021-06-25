---
layout: default
title: "test"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="test">
  <a href="/en/common/test.html">test</a> <a href="#test"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Evaluate condition.
> Returns 0 if the condition evaluates to true, 1 if it evaluates to false.
> More information: <https://www.gnu.org/software/coreutils/test>.

#### Test if a given variable is equal to a given string:
```shell
test "{{$MY_VAR}}" == "{{/bin/zsh}}"
```
#### Test if a given variable is empty:
```shell
test -z "{{$GIT_BRANCH}}"
```
#### Test if a file exists:
```shell
test -f "{{path/to/file_or_directory}}"
```
#### Test if a directory does not exist:
```shell
test ! -d "{{path/to/directory}}"
```
#### If-else statement:
```shell
test {{condition}} && {{echo "true"}} || {{echo "false"}}
```
{% endraw %}