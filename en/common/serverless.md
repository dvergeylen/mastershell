---
layout: default
title: "serverless"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="serverless">
  <a href="/en/common/serverless.html">serverless</a> <a href="#serverless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Toolkit for deploying and operating serverless architectures on AWS, Google Cloud, Azure and IBM OpenWhisk.
> Commands can be run either using the `serverless` command or it's alias, `sls`.
> More information: <https://serverless.com/>.

#### Create a serverless project:
```shell
serverless create
```
#### Create a serverless project from a template:
```shell
serverless create --template {{template_name}}
```
#### Deploy to a cloud provider:
```shell
serverless deploy
```
#### Display information about a serverless project:
```shell
serverless info
```
#### Invoke a deployed function:
```shell
serverless invoke -f {{function_name}}
```
#### Follow the logs for a project:
```shell
serverless logs -t
```
{% endraw %}