---
layout: default
title: "aws quicksight"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-quicksight">
  <a href="/de/common/aws-quicksight.html">aws quicksight</a> <a href="#aws-quicksight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI für AWS QuickSight.
> Weitere Informationen: <https://docs.aws.amazon.com/cli/latest/reference/quicksight/>.

#### Liste alle Datensätze auf:
```shell
aws quicksight list-data-sets --aws-account-id {{aws_account_id}}
```
#### Liste alle Benutzer auf:
```shell
aws quicksight list-users --aws-account-id {{aws_account_id}} --namespace default
```
#### Liste alle Gruppen auf:
```shell
aws quicksight list-groups --aws-account-id {{aws_account_id}} --namespace default
```
#### Liste alle Dashboards auf:
```shell
aws quicksight list-dashboards --aws-account-id {{aws_account_id}}
```
#### Liste eine Datensatz detailliert aus:
```shell
aws quicksight describe-data-set --aws-account-id {{aws_account_id}} --data-set-id {{datensatz_id}}
```
#### Liste Zugangsberechtungen zu einem Datensatz auf:
```shell
aws quicksight describe-data-set-permissions --aws-account-id {{aws_account_id}} --data-set-id {{datensatz_id}}
```
{% endraw %}