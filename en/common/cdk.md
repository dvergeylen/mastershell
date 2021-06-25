---
layout: default
title: "cdk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cdk">
  <a href="/en/common/cdk.html">cdk</a> <a href="#cdk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI for AWS Cloud Development Kit (CDK).
> More information: <https://docs.aws.amazon.com/cdk/latest/guide/cli.html>.

#### List the stacks in the app:
```shell
cdk ls
```
#### Synthesize and print the CloudFormation template for the specified stack(s):
```shell
cdk synth {{stack_name}}
```
#### Deploy a space-separated list of stacks:
```shell
cdk deploy {{stack_name}}
```
#### Destroy a space-separated list of stacks:
```shell
cdk destroy {{stack_name}}
```
#### Compare the specified stack with the deployed stack or a local CloudFormation template:
```shell
cdk diff {{stack_name}}
```
#### Create a new CDK project in the current directory for a specified language:
```shell
cdk init -l {{language_name}}
```
#### Open the CDK API reference in your browser:
```shell
cdk doc
```
{% endraw %}