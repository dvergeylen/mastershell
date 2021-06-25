---
layout: default
title: "aws iam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-iam">
  <a href="/en/common/aws-iam.html">aws iam</a> <a href="#aws-iam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for AWS IAM.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/iam/index.html>.

#### Show `aws iam` help page (including all available iam commands):
```shell
aws iam help
```
#### List users:
```shell
aws iam list-users
```
#### List policies:
```shell
aws iam list-policies
```
#### List groups:
```shell
aws iam list-groups
```
#### Get users in a group:
```shell
aws iam get-group --group-name {{group_name}}
```
#### Describe an IAM policy:
```shell
aws iam get-policy --policy-arn arn:aws:iam::aws:policy/{{policy_name}}
```
#### List access keys:
```shell
aws iam list-access-keys
```
#### List access keys for a specific user:
```shell
aws iam list-access-keys --user-name {{user_name}}
```
{% endraw %}