---
layout: default
title: "ng"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ng">
  <a href="/en/common/ng.html">ng</a> <a href="#ng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line Interface (CLI) for creating and managing Angular applications.
> More information: <https://angular.io/cli>.

#### Create a new Angular application inside a directory:
```shell
ng new {{project_name}}
```
#### Add a new component to one's application:
```shell
ng generate component {{component_name}}
```
#### Add a new class to one's application:
```shell
ng generate class {{class_name}}
```
#### Add a new directive to one's application:
```shell
ng generate directive {{directive_name}}
```
#### Run the application with the following command in its root directory:
```shell
ng serve
```
#### Build the application:
```shell
ng build
```
#### Run unit tests:
```shell
ng test
```
#### Check the version of your current Angular installation:
```shell
ng version
```
{% endraw %}