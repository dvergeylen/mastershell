---
layout: default
title: "github-label-sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="github-label-sync">
  <a href="/en/common/github-label-sync.html">github-label-sync</a> <a href="#github-label-sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface for synchronising GitHub labels.
> More information: <https://npmjs.com/package/github-label-sync>.

#### Synchronise labels using a local `labels.json` file:
```shell
github-label-sync --access-token {{token}} {{repository_name}}
```
#### Synchronise labels using a specific labels JSON file:
```shell
github-label-sync --access-token {{token}} --labels {{url|path/to/json_file}} {{repository_name}}
```
#### Perform a dry run instead of actually synchronising labels:
```shell
github-label-sync --access-token {{token}} --dry-run {{repository_name}}
```
#### Keep labels that aren't in `labels.json`:
```shell
github-label-sync --access-token {{token}} --allow-added-labels {{repository_name}}
```
#### Synchronise using the `GITHUB_ACCESS_TOKEN` environment variable:
```shell
github-label-sync {{repository_name}}
```
{% endraw %}