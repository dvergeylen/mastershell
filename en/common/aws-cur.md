---
layout: default
title: "aws cur"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-cur">
  <a href="/en/common/aws-cur.html">aws cur</a> <a href="#aws-cur"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, query, and delete AWS usage report definitions.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/cur/index.html>.

#### Create an AWS cost and usage report definition from a JSON file:
```shell
aws cur put-report-definition --report-definition file://{{path/to/report-definition.json}}
```
#### List usage report definitions defined for the logged in account:
```shell
aws cur describe-report-definitions
```
#### Delete a usage report definition:
```shell
aws cur --region {{aws_region}} delete-report-definition --report-name {{report}}
```
{% endraw %}