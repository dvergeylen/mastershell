---
layout: default
title: "django-admin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="django-admin">
  <a href="/en/common/django-admin.html">django-admin</a> <a href="#django-admin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Django’s utility for administrative tasks.
> More information: <https://docs.djangoproject.com/en/3.0/ref/django-admin/>.

#### Create a new django project:
```shell
django-admin startproject {{project_name}}
```
#### Create a new app for the current project:
```shell
django-admin startapp {{app_name}}
```
#### Check the current version of Django:
```shell
django-admin --version
```
#### Display more information for the given command:
```shell
django-admin help {{command}}
```
{% endraw %}