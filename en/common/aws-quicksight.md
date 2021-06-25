---
layout: default
title: "aws quicksight"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-quicksight">
  <a href="/en/common/aws-quicksight.html">aws quicksight</a> <a href="#aws-quicksight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for AWS QuickSight.
> Access QuickSight entities.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/quicksight/>.

#### List datasets:
```shell
aws quicksight list-data-sets --aws-account-id {{aws_account_id}}
```
#### List users:
```shell
aws quicksight list-users --aws-account-id {{aws_account_id}} --namespace default
```
#### List groups:
```shell
aws quicksight list-groups --aws-account-id {{aws_account_id}} --namespace default
```
#### List dashboards:
```shell
aws quicksight list-dashboards --aws-account-id {{aws_account_id}}
```
#### Display detailed information about a dataset:
```shell
aws quicksight describe-data-set --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}
```
#### Display who has access to the dataset and what kind of actions they can perform on the dataset:
```shell
aws quicksight describe-data-set-permissions --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}
```
{% endraw %}