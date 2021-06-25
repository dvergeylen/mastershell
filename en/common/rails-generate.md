---
layout: default
title: "rails generate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails-generate">
  <a href="/en/common/rails-generate.html">rails generate</a> <a href="#rails-generate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate new Rails templates in an existing project.
> More information: <https://guides.rubyonrails.org/command_line.html#bin-rails-generate>.

#### List all available generators:
```shell
rails generate
```
#### Generate a new model named Post with attributes title and body:
```shell
rails generate model {{Post}} {{title:string}} {{body:text}}
```
#### Generate a new controller named Posts with actions index, show, new and create:
```shell
rails generate controller {{Posts}} {{index}} {{show}} {{new}} {{create}}
```
#### Generate a new migration that adds a category attribute to an existing model called Post:
```shell
rails generate migration {{AddCategoryToPost}} {{category:string}}
```
#### Generate a scaffold for a model named Post, predefining the attributes title and body:
```shell
rails generate scaffold {{Post}} {{title:string}} {{body:text}}
```
{% endraw %}