---
layout: default
title: "exenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exenv">
  <a href="/en/common/exenv.html">exenv</a> <a href="#exenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to easily install Elixir versions and manage application environments.
> More information: <https://github.com/exenv/exenv>.

#### Display a list of installed versions:
```shell
exenv versions
```
#### Use a specific version of Elixir across the whole system:
```shell
exenv global {{version}}
```
#### Use a specific version of Elixir for the current application/project directory:
```shell
exenv local {{version}}
```
#### Show the currently selected Elixir version:
```shell
exenv {{version}}
```
#### Install a version of Elixir (requires `elixir-build` plugin <https://github.com/mururu/elixir-build>):
```shell
exenv install {{version}}
```
{% endraw %}