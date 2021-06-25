---
layout: default
title: "awslogs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="awslogs">
  <a href="/de/common/awslogs.html">awslogs</a> <a href="#awslogs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI um Log-Gruppen, Streams und Events von Amazon CloudWatch Logs abzurufen.
> Weitere Informationen: <https://github.com/jorgebastida/awslogs>.

#### Liste alle Log-Gruppen auf:
```shell
awslogs groups
```
#### Liste alle bestehenden Streams einer angegebenen Log Gruppe auf:
```shell
awslogs streams {{/var/log/syslog}}
```
#### Rufe alle logs für jegliche Streams in der angegebenen Log-Gruppe für die letzten 1 bis 2 Stunden ab:
```shell
awslogs get {{/var/log/syslog}} --start='{{2h ago}}' --end='{{1h ago}}'
```
#### Rufe alle Logs für einen bestimmten CloudWatch-Logs Filter-Ausdruck ab:
```shell
awslogs get {{/aws/lambda/meine_lambda_gruppe}} --filter-pattern='{{ERROR}}'
```
#### Beobachte Logs für jegliche Streams in der angegebenen Log-Gruppe:
```shell
awslogs get {{/var/log/syslog}} ALL --watch
```
{% endraw %}