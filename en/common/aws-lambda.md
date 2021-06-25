---
layout: default
title: "aws lambda"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-lambda">
  <a href="/en/common/aws-lambda.html">aws lambda</a> <a href="#aws-lambda"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for AWS lambda.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/lambda/>.

#### Run a function:
```shell
aws lambda invoke --function-name {{name}} {{path/to/response}}.json
```
#### Run a function with an input payload in JSON format:
```shell
aws lambda invoke --function-name {{name}} --payload {{json}} {{path/to/response}}.json
```
#### List functions:
```shell
aws lambda list-functions
```
#### Display the configuration of a function:
```shell
aws lambda get-function-configuration --function-name {{name}}
```
#### List function aliases:
```shell
aws lambda list-aliases --function-name {{name}}
```
#### Display the reserved concurrency configuration for a function:
```shell
aws lambda get-function-concurrency --function-name {{name}}
```
#### List which AWS services can invoke the function:
```shell
aws lambda get-policy --function-name {{name}}
```
{% endraw %}