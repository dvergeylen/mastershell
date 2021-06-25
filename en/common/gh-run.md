---
layout: default
title: "gh run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-run">
  <a href="/en/common/gh-run.html">gh run</a> <a href="#gh-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View, run and watch recent GitHub Actions workflow runs.
> More information: <https://cli.github.com/manual/gh_run>.

#### Interactively select a run to see information about the jobs:
```shell
gh run view
```
#### Display information about a specific run:
```shell
gh run view {{workflow_run_number}}
```
#### Display information about the steps of a job:
```shell
gh run view --job={{job_number}}
```
#### Display the log of a job:
```shell
gh run view --job={{job_number}} --log
```
#### Check a specific workflow and exit with a non-zero status if the run failed:
```shell
gh run view {{workflow_run_number}} --exit-status && {{echo "run pending or passed"}}
```
#### Interactively select an active run and wait until it's done:
```shell
gh run watch
```
#### Display the jobs for a run and wait until it's done:
```shell
gh run watch {{workflow_run_number}}
```
#### Re-run a specific workflow:
```shell
gh run rerun {{workflow_run_number}}
```
{% endraw %}