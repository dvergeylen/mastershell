---
layout: default
title: "docker exec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-exec">
  <a href="/en/common/docker-exec.html">docker exec</a> <a href="#docker-exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute a command on an already running Docker container.
> More information: <https://docs.docker.com/engine/reference/commandline/exec/>.

#### Enter an interactive shell session on an already-running container:
```shell
docker exec --interactive --tty {{container_name}} {{/bin/bash}}
```
#### Run a command in the background (detached) on a running container:
```shell
docker exec --detach {{container_name}} {{command}}
```
#### Select the working directory for a given command to execute into:
```shell
docker exec --interactive -tty --workdir {{path/to/directory}} {{container_name}} {{command}}
```
#### Run a command in background on existing container but keep stdin open:
```shell
docker exec --interactive --detach {{container_name}} {{command}}
```
#### Set an environment variable in a running bash session:
```shell
docker exec --interactive --tty --env {{variable_name}}={{value}} {{container_name}} {{/bin/bash}}
```
#### Run a command as a specific user:
```shell
docker exec --user {{user}} {{container_name}} {{command}}
```
{% endraw %}