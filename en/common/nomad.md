---
layout: default
title: "nomad"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nomad">
  <a href="/en/common/nomad.html">nomad</a> <a href="#nomad"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Distributed, highly available, datacenter-aware scheduler.
> More information: <https://www.nomadproject.io/docs/commands/>.

#### Show the status of nodes in the cluster:
```shell
nomad node status
```
#### Validate a job file:
```shell
nomad job validate {{path/to/file.nomad}}
```
#### Plan a job for execution on the cluster:
```shell
nomad job plan {{path/to/file.nomad}}
```
#### Run a job on the cluster:
```shell
nomad job run {{path/to/file.nomad}}
```
#### Show the status of jobs currently running on the cluster:
```shell
nomad job status
```
#### Show the detailed status information about a specific job:
```shell
nomad job status {{job_name}}
```
#### Follow the logs of a specific allocation:
```shell
nomad alloc logs {{alloc_id}}
```
#### Show the status of storage volumes:
```shell
nomad volume status
```
{% endraw %}