---
layout: default
title: "docker stats"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-stats">
  <a href="/en/common/docker-stats.html">docker stats</a> <a href="#docker-stats"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a live stream of resource usage statistics for containers.
> More information: <https://docs.docker.com/engine/reference/commandline/stats/>.

#### Display a live stream for the statistics of all running containers:
```shell
docker stats
```
#### Display a live stream of statistics for a space-separated list of containers:
```shell
docker stats {{container_name}}
```
#### Change the columns format to display container's cpu usage percentage:
```shell
docker stats --format "{{.Name}}:\t{{.CPUPerc}}"
```
#### Display statistics for all containers (both running and stopped):
```shell
docker stats --all
```
#### Disable streaming stats and only pull the current stats:
```shell
docker stats --no-stream
```
{% endraw %}