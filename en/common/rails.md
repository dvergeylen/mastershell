---
layout: default
title: "rails"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails">
  <a href="/en/common/rails.html">rails</a> <a href="#rails"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A server-side MVC framework written in Ruby.
> More information: <https://guides.rubyonrails.org/command_line.html>.

#### Create a new rails project:
```shell
rails new "{{project_name}}"
```
#### Start local server for current project on port 3000:
```shell
rails server
```
#### Start local server for current project on a specified port:
```shell
rails server -p "{{port}}"
```
#### Open console to interact with application from command-line:
```shell
rails console
```
#### Check current version of rails:
```shell
rails --version
```
{% endraw %}