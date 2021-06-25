---
layout: default
title: "aws"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws">
  <a href="/en/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The official CLI tool for Amazon Web Services.
> Wizard, SSO, Resource Autocompletion, and YAML options are v2 only.
> More information: <https://aws.amazon.com/cli>.

#### Configure the AWS Command-line:
```shell
aws configure wizard
```
#### Configure the AWS Command-line using SSO:
```shell
aws configure sso
```
#### See help text for the AWS command:
```shell
aws {{command}} help
```
#### Get the caller identity (used to troubleshoot permissions):
```shell
aws sts get-caller-identity
```
#### List AWS resources in a region and output in yaml:
```shell
aws dynamodb list-tables --region {{us-east-1}} --output yaml
```
#### Use auto prompt to help with a command:
```shell
aws iam create-user --cli-auto-prompt
```
#### Get an interactive wizard for an AWS resource:
```shell
aws dynamodb wizard {{new_table}}
```
#### Generate a JSON CLI Skeleton (useful for infrastructure as code):
```shell
aws dynamodb update-table --generate-cli-skeleton
```
{% endraw %}