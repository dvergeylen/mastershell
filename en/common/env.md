---
layout: default
title: "env"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="env">
  <a href="/en/common/env.html">env</a> <a href="#env"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the environment or run a program in a modified environment.
> More information: <https://www.gnu.org/software/coreutils/env>.

#### Show the environment:
```shell
env
```
#### Run a program. Often used in scripts after the shebang (#!) for looking up the path to the program:
```shell
env {{program}}
```
#### Clear the environment and run a program:
```shell
env -i {{program}}
```
#### Remove variable from the environment and run a program:
```shell
env -u {{variable}} {{program}}
```
#### Set a variable and run a program:
```shell
env {{variable}}={{value}} {{program}}
```
#### Set multiple variables and run a program:
```shell
env {{variable1}}={{value}} {{variable2}}={{value}} {{variable3}}={{value}} {{program}}
```
{% endraw %}