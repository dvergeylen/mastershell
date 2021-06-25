---
layout: default
title: "rails destroy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails-destroy">
  <a href="/en/common/rails-destroy.html">rails destroy</a> <a href="#rails-destroy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Destroy Rails resources.
> More information: <https://guides.rubyonrails.org/command_line.html#bin-rails-destroy>.

#### List all available generators to destroy:
```shell
rails destroy
```
#### Destroy a model named Post:
```shell
rails destroy model {{Post}}
```
#### Destroy a controller named Posts:
```shell
rails destroy controller {{Posts}}
```
#### Destroy a migration that creates Posts:
```shell
rails destroy migration {{CreatePosts}}
```
#### Destroy a scaffold for a model named Post:
```shell
rails destroy scaffold {{Post}}
```
{% endraw %}