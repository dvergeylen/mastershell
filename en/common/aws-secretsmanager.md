---
layout: default
title: "aws secretsmanager"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-secretsmanager">
  <a href="/en/common/aws-secretsmanager.html">aws secretsmanager</a> <a href="#aws-secretsmanager"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Store, manage, and retrieve secrets.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/secretsmanager/>.

#### Show secrets stored by the secrets manager in the current account:
```shell
aws secretsmanager list-secrets
```
#### Create a secret:
```shell
aws secretsmanager create-secret --name {{name}} --description "{{secret_description}}" --secret-string {{secret}}
```
#### Delete a secret:
```shell
aws secretsmanager delete-secret --secret-id {{name_or_arn}}
```
#### View details of a secret except for secret text:
```shell
aws secretsmanager describe-secret --secret-id {{name_or_arn}}
```
#### Retrieve the value of a secret (to get the latest version of the secret omit `--version-stage`):
```shell
aws secretsmanager get-secret-value --secret-id {{name_or_arn}} --version-stage {{version_of_secret}}
```
#### Rotate the secret immediately using a Lambda function:
```shell
aws secretsmanager rotate-secret --secret-id {{name_or_arn}} --rotation-lambda-arn {{arn_of_lambda_function}}
```
#### Rotate the secret automatically every 30 days using a Lambda function:
```shell
aws secretsmanager rotate-secret --secret-id {{name_or_arn}} --rotation-lambda-arn {{arn_of_lambda_function}} --rotation-rules AutomaticallyAfterDays={{30}}
```
{% endraw %}