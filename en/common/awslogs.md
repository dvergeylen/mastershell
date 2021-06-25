---
layout: default
title: "awslogs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="awslogs">
  <a href="/en/common/awslogs.html">awslogs</a> <a href="#awslogs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Queries groups, streams and events from Amazon CloudWatch logs.
> More information: <https://github.com/jorgebastida/awslogs>.

#### List log groups:
```shell
awslogs groups
```
#### List existing streams for the specified group:
```shell
awslogs streams {{/var/log/syslog}}
```
#### Get logs for any streams in the specified group between 1 and 2 hours ago:
```shell
awslogs get {{/var/log/syslog}} --start='{{2h ago}}' --end='{{1h ago}}'
```
#### Get logs that match a specific CloudWatch Logs Filter pattern:
```shell
awslogs get {{/aws/lambda/my_lambda_group}} --filter-pattern='{{ERROR}}'
```
#### Watch logs for any streams in the specified group:
```shell
awslogs get {{/var/log/syslog}} ALL --watch
```
{% endraw %}