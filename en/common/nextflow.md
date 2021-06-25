---
layout: default
title: "nextflow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nextflow">
  <a href="/en/common/nextflow.html">nextflow</a> <a href="#nextflow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for running computational pipelines. Mostly used for bioinformatics workflows.
> More information: <https://www.nextflow.io>.

#### Run a pipeline, use cached results from previous runs:
```shell
nextflow run {{main.nf}} -resume
```
#### Run a specific release of a remote workflow from GitHub:
```shell
nextflow run {{user/repo}} -revision {{release_tag}}
```
#### Run with a given work directory for intermediate files, save execution report:
```shell
nextflow run {{workflow}} -work-dir {{path/to/directory}} -with-report {{report.html}}
```
#### Show details of previous runs in current directory:
```shell
nextflow log
```
#### Remove cache and intermediate files for a specific run:
```shell
nextflow clean -force {{run_name}}
```
#### List all downloaded projects:
```shell
nextflow list
```
#### Pull the latest version of a remote workflow from Bitbucket:
```shell
nextflow pull {{user/repo}} -hub bitbucket
```
#### Update Nextflow:
```shell
nextflow self-update
```
{% endraw %}