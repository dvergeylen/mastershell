---
layout: default
title: "gitlab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gitlab">
  <a href="/en/common/gitlab.html">gitlab</a> <a href="#gitlab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ruby wrapper and CLI for the GitLab API.
> More information: <https://narkoz.github.io/gitlab/>.

#### Create a new project:
```shell
gitlab create_project {{project_name}}
```
#### Get info about a specific commit:
```shell
gitlab commit {{project_name}} {{commit_hash}}
```
#### Get info about jobs in a CI pipeline:
```shell
gitlab pipeline_jobs {{project_name}} {{pipeline_id}}
```
#### Start a specific CI job:
```shell
gitlab job_play {{project_name}} {{job_id}}
```
{% endraw %}