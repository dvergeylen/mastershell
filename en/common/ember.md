---
layout: default
title: "ember"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ember">
  <a href="/en/common/ember.html">ember</a> <a href="#ember"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Ember.js command-line utility.
> Used for creating and maintaining Ember.js applications.
> More information: <https://cli.emberjs.com>.

#### Create a new Ember application:
```shell
ember new {{my_new_app}}
```
#### Create a new Ember addon:
```shell
ember addon {{my_new_addon}}
```
#### Build the project:
```shell
ember build
```
#### Build the project in production mode:
```shell
ember build -prod
```
#### Run the development server:
```shell
ember serve
```
#### Run the test suite:
```shell
ember test
```
#### Run a blueprint to generate something like a route or component:
```shell
ember generate {{type}} {{name}}
```
#### Install an ember-cli addon:
```shell
ember install {{name_of_addon}}
```
{% endraw %}