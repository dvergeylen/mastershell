---
layout: default
title: "drupal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drupal">
  <a href="/en/common/drupal.html">drupal</a> <a href="#drupal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for Drupal.
> Generates boilerplate code, interacts with and debugs Drupal projects.
> More information: <https://drupalconsole.com/>.

#### Install a module:
```shell
drupal module:install {{module_name}}
```
#### Uninstall a module:
```shell
drupal module:uninstall {{module_name}}
```
#### Clear all caches:
```shell
drupal cache:rebuild
```
#### View current Drupal installation status:
```shell
drupal site:status
```
{% endraw %}