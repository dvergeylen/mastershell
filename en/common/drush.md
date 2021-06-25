---
layout: default
title: "drush"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drush">
  <a href="/en/common/drush.html">drush</a> <a href="#drush"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line shell and scripting interface for Drupal.
> More information: <https://www.drush.org>.

#### Enable module "foo":
```shell
drush en {{foo}}
```
#### Uninstall module "foo":
```shell
drush pmu {{foo}}
```
#### Clear all caches:
```shell
drush cr
```
#### Clear CSS and JavaScript caches:
```shell
drush cc css-js
```
{% endraw %}