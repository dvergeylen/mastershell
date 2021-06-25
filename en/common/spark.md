---
layout: default
title: "spark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spark">
  <a href="/en/common/spark.html">spark</a> <a href="#spark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Laravel Spark command-line tool.
> More information: <https://spark.laravel.com>.

#### Register your API token:
```shell
spark register {{token}}
```
#### Display the currently registered API token:
```shell
spark token
```
#### Create a new Spark project:
```shell
spark new {{project_name}}
```
#### Create a new Spark project with Braintree stubs:
```shell
spark new {{project_name}} --braintree
```
#### Create a new Spark project with team based billing stubs:
```shell
spark new {{project_name}} --team-billing
```
{% endraw %}