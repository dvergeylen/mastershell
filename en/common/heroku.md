---
layout: default
title: "heroku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="heroku">
  <a href="/en/common/heroku.html">heroku</a> <a href="#heroku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manage Heroku apps from the command-line.
> More information: <https://www.heroku.com/>.

#### Log in to your heroku account:
```shell
heroku login
```
#### Create a heroku app:
```shell
heroku create
```
#### Show logs for an app:
```shell
heroku logs --app {{app_name}}
```
#### Run a one-off process inside a dyno (Heroku virtual machine):
```shell
heroku run {{process_name}} --app {{app_name}}
```
#### List dynos (Heroku virtual machines) for an app:
```shell
heroku ps --app {{app_name}}
```
#### Permanently destroy an app:
```shell
heroku destroy --app {{app_name}}
```
{% endraw %}