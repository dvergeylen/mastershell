---
layout: default
title: "fly"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fly">
  <a href="/en/common/fly.html">fly</a> <a href="#fly"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool for concourse-ci.
> More information: <https://concourse-ci.org/fly.html>.

#### Authenticate with and save concourse target:
```shell
fly --target {{target_name}} login --team-name {{team_name}} -c {{https://ci.example.com}}
```
#### List targets:
```shell
fly targets
```
#### List pipelines:
```shell
fly -t {{target_name}} pipelines
```
#### Upload or update a pipeline:
```shell
fly -t {{target_name}} set-pipeline --config {{pipeline.yml}} --pipeline {{pipeline_name}}
```
#### Unpause pipeline:
```shell
fly -t {{target_name}} unpause-pipeline --pipeline {{pipeline_name}}
```
#### Show pipeline configuration:
```shell
fly -t {{target_name}} get-pipeline --pipeline {{pipeline_name}}
```
#### Update local copy of fly:
```shell
fly -t {{target_name}} sync
```
#### Destroy pipeline:
```shell
fly -t {{target_name}} destroy-pipeline --pipeline {{pipeline_name}}
```
{% endraw %}