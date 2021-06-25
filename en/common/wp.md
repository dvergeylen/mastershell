---
layout: default
title: "wp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wp">
  <a href="/en/common/wp.html">wp</a> <a href="#wp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The official command-line interface to manage WordPress instances.
> More information: <https://wp-cli.org/>.

#### Print information about the operating system, shell, PHP, and WP-CLI (`wp`) installation:
```shell
wp --info
```
#### Update WP-CLI:
```shell
wp cli update
```
#### Install and activate a WordPress plugin:
```shell
wp plugin install {{plugin}} --activate
```
#### Replace all instances of a string in the database:
```shell
wp search-replace {{old_string}} {{new_string}}
```
#### Import the contents of a WordPress Extended RSS (WXR) file:
```shell
wp import {{path/to/file.xml}}
```
{% endraw %}