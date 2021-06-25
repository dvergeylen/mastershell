---
layout: default
title: "aws glue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-glue">
  <a href="/en/common/aws-glue.html">aws glue</a> <a href="#aws-glue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for AWS Glue.
> Defines the public endpoint for the AWS Glue service.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/glue/>.

#### List jobs:
```shell
aws glue list-jobs
```
#### Start a job:
```shell
aws glue start-job-run --job-name {{job_name}}
```
#### Start running a workflow:
```shell
aws glue start-workflow-run --name {{workflow_name}}
```
#### List triggers:
```shell
aws glue list-triggers
```
#### Start a trigger:
```shell
aws glue start-trigger --name {{trigger_name}}
```
#### Create a dev endpoint:
```shell
aws glue create-dev-endpoint --endpoint-name {{name}} --role-arn {{role_arn_used_by_endpoint}}
```
{% endraw %}