---
layout: default
title: "meteor"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="meteor">
  <a href="/en/common/meteor.html">meteor</a> <a href="#meteor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Full-stack JavaScript platform for building web applications.
> More information: <https://meteor.com>.

#### Run a meteor project from its root directory in development mode:
```shell
meteor
```
#### Create a project under the given directory:
```shell
meteor create {{path/to/directory}}
```
#### Display the list of packages the project is currently using:
```shell
meteor list
```
#### Add a package to the project:
```shell
meteor add {{package_name}}
```
#### Remove a package from the project:
```shell
meteor remove {{package_name}}
```
#### Create a production build of the project as a tarball under the given directory:
```shell
meteor build {{path/to/directory}}
```
{% endraw %}