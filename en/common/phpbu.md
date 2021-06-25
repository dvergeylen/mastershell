---
layout: default
title: "phpbu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpbu">
  <a href="/en/common/phpbu.html">phpbu</a> <a href="#phpbu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A backup utility framework for PHP.
> More information: <https://phpbu.de>.

#### Run backups using the default `phpbu.xml` configuration file:
```shell
phpbu
```
#### Run backups using a specific configuration file:
```shell
phpbu --configuration={{path/to/configuration_file.xml}}
```
#### Only run the specified backups:
```shell
phpbu --limit={{backup_task_name}}
```
#### Simulate the actions that would have been performed:
```shell
phpbu --simulate
```
{% endraw %}