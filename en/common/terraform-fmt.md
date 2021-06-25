---
layout: default
title: "terraform fmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="terraform-fmt">
  <a href="/en/common/terraform-fmt.html">terraform fmt</a> <a href="#terraform-fmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Format configuration according to Terraform language style conventions.
> More information: <https://www.terraform.io/docs/commands/fmt.html>.

#### Format the configuration in the current directory:
```shell
terraform fmt
```
#### Format the configuration in the current directory and subdirectories:
```shell
terraform fmt -recursive
```
#### Display diffs of formatting changes:
```shell
terraform fmt -diff
```
#### Do not list files that were formatted to stdout:
```shell
terraform fmt -list=false
```
{% endraw %}