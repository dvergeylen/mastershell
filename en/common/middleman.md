---
layout: default
title: "middleman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="middleman">
  <a href="/en/common/middleman.html">middleman</a> <a href="#middleman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Static site generator written in Ruby.
> More information: <https://middlemanapp.com/>.

#### Create a new Middleman project:
```shell
middleman init "{{project_name}}"
```
#### Start local server for current project on port 4567:
```shell
middleman server
```
#### Start local server for current project on a specified port:
```shell
middleman server -p "{{port}}"
```
#### Build the project in the current directory to prepare for deployment:
```shell
bundle exec middleman build
```
#### Deploy the Middleman project in the current directory:
```shell
middleman deploy
```
{% endraw %}