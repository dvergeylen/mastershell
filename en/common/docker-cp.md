---
layout: default
title: "docker cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-cp">
  <a href="/en/common/docker-cp.html">docker cp</a> <a href="#docker-cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files or directories between host and container filesystems.
> More information: <https://docs.docker.com/engine/reference/commandline/cp>.

#### Copy a file or directory from the host to a container:
```shell
docker cp {{path/to/file_or_directory_on_host}} {{container_name}}:{{path/to/file_or_directory_in_container}}
```
#### Copy a file or directory from a container to the host:
```shell
docker cp {{container_name}}:{{path/to/file_or_directory_in_container}} {{path/to/file_or_directory_on_host}}
```
#### Copy a file or directory from the host to a container, following symlinks (copies the symlinked files directly, not the symlinks themselves):
```shell
docker cp --follow-link {{path/to/symlink_on_host}} {{container_name}}:{{path/to/file_or_directory_in_container}}
```
{% endraw %}