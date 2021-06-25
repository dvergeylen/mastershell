---
layout: default
title: "vue init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vue-init">
  <a href="/en/common/vue-init.html">vue init</a> <a href="#vue-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Legacy project initialization subcommand of the Vue.js framework.
> More information: <https://cli.vuejs.org/guide/creating-a-project.html#pulling-2-x-templates-legacy>.

#### Create a new project using one of the default templates:
```shell
vue init {{webpack|webpack-simple|browserify|browserify-simple|simple}} {{project_name}}
```
#### Create a new project using a local template:
```shell
vue init {{path/to/template_directory}} {{project_name}}
```
#### Create a new project using a template from GitHub:
```shell
vue init {{username}}/{{repo}} {{project_name}}
```
{% endraw %}