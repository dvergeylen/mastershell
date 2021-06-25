---
layout: default
title: "act"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="act">
  <a href="/en/common/act.html">act</a> <a href="#act"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute GitHub Actions locally using Docker.
> More information: <https://github.com/nektos/act>.

#### List the available actions:
```shell
act -l
```
#### Run the default event:
```shell
act
```
#### Run a specific event:
```shell
act {{event_type}}
```
#### Run a specific action:
```shell
act -a {{action_id}}
```
#### Do not actually run the actions (i.e. a dry run):
```shell
act -n
```
#### Show verbose logs:
```shell
act -v
```
{% endraw %}