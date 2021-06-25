---
layout: default
title: "rails routes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails-routes">
  <a href="/en/common/rails-routes.html">rails routes</a> <a href="#rails-routes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List routes in a Rails application.
> More information: <https://guides.rubyonrails.org/routing.html>.

#### List all routes:
```shell
rails routes
```
#### List all routes in an expanded format:
```shell
rails routes --expanded
```
#### List routes partially matching URL helper method name, HTTP verb, or URL path:
```shell
rails routes -g {{posts_path|GET|/posts}}
```
#### List routes that map to a specified controller:
```shell
rails routes -c {{posts|Posts|Blogs::PostsController}}
```
{% endraw %}