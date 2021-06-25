---
layout: default
title: "jobs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jobs">
  <a href="/en/common/jobs.html">jobs</a> <a href="#jobs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display status of jobs in the current session.

#### Show status of all jobs:
```shell
jobs
```
#### Show status of a particular job:
```shell
jobs %{{job_id}}
```
#### Show status and process IDs of all jobs:
```shell
jobs -l
```
#### Show process IDs of all jobs:
```shell
jobs -p
```
{% endraw %}