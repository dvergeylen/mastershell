---
layout: default
title: "gh workflow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-workflow">
  <a href="/en/common/gh-workflow.html">gh workflow</a> <a href="#gh-workflow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List, view, and run GitHub Actions workflows.
> More information: <https://cli.github.com/manual/gh_workflow>.

#### Interactively select a workflow to view the latest jobs for:
```shell
gh workflow view
```
#### View a specific workflow in the default browser:
```shell
gh workflow view {{id|workflow_name|filename.yml}} --web
```
#### Display the YAML definition of a specific workflow:
```shell
gh workflow view {{id|workflow_name|filename.yml}} --yaml
```
#### Display the YAML definition for a specific Git branch or tag:
```shell
gh workflow view {{id|workflow_name|filename.yml}} --ref {{branch_or_tag_name}} --yaml
```
#### List workflow files (use `--all` to include disabled workflows):
```shell
gh workflow list
```
#### Run a manual workflow with parameters:
```shell
gh workflow run {{id|workflow_name|filename.yml}} --raw-field {{param1}}={{value1}} --raw-field {{param2}}={{value2}}
```
#### Run a manual workflow using a specific branch or tag with JSON parameters from stdin:
```shell
echo '{{{"param1":"value1", "param2":"value2"}}}' | gh workflow run {{id|workflow_name|filename.yml}} --ref {{branch_or_tag_name}}
```
#### Enable or disable a specific workflow:
```shell
gh workflow {{enable|disable}} {{id|workflow_name|filename.yml}}
```
{% endraw %}