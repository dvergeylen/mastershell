---
layout: default
title: "docker login"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-login">
  <a href="/en/common/docker-login.html">docker login</a> <a href="#docker-login"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Log into a docker registry.
> More information: <https://docs.docker.com/engine/reference/commandline/login/>.

#### Interactively log into a registry:
```shell
docker login
```
#### Log into a registry with a specific username (user will be prompted for a password):
```shell
docker login --username {{username}}
```
#### Log into a registry with username and password:
```shell
docker login --username {{username}} --password {{password}} {{server}}
```
#### Log into a registry with password from stdin:
```shell
 echo "{{password}}" | docker login --username {{username}} --password-stdin
```
{% endraw %}