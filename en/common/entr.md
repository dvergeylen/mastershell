---
layout: default
title: "entr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="entr">
  <a href="/en/common/entr.html">entr</a> <a href="#entr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run arbitrary commands when files change.
> More information: <https://manned.org/entr>.

#### Rebuild with `make` if any file in any subdirectory changes:
```shell
{{ag -l}} | entr {{make}}
```
#### Rebuild and test with `make` if any `.c` source files in the current directory change:
```shell
{{ls *.c}} | entr {{'make && make test'}}
```
#### Send a `SIGTERM` to any previously spawned ruby subprocesses before executing `ruby main.rb`:
```shell
{{ls *.rb}} | entr -r {{ruby main.rb}}
```
#### Run a command with the changed file (`/_`) as an argument:
```shell
{{ls *.sql}} | entr {{psql -f}} /_
```
{% endraw %}