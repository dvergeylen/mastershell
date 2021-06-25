---
layout: default
title: "docker secret"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-secret">
  <a href="/en/common/docker-secret.html">docker secret</a> <a href="#docker-secret"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Docker swarm secrets.
> More information: <https://docs.docker.com/engine/reference/commandline/secret/>.

#### Create a new secret from stdin:
```shell
{{command}} | docker secret create {{secret_name}} -
```
#### Create a new secret from a file:
```shell
docker secret create {{secret_name}} {{path/to/file}}
```
#### List all secrets:
```shell
docker secret ls
```
#### Display detailed information on one or multiple secrets in a human friendly format:
```shell
docker secret inspect --pretty {{secret_name1 secret_name2 ...}}
```
#### Remove one or more secrets:
```shell
docker secret rm {{secret_name1 secret_name2 ...}}
```
{% endraw %}