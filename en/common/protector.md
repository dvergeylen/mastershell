---
layout: default
title: "protector"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="protector">
  <a href="/en/common/protector.html">protector</a> <a href="#protector"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Protect or unprotect branches on GitHub repositories.
> More information: <https://github.com/jcgay/protector>.

#### Protect branches of a GitHub repository (create branch protection rules):
```shell
protector {{branches_regex}} -repos {{organization/repository}}
```
#### Use the dry run to see what would be protected (can also be used for freeing):
```shell
protector -dry-run {{branches_regex}} -repos {{organization/repository}}
```
#### Free branches of a GitHub repository (delete branch protection rules):
```shell
protector -free {{branches_regex}} -repos {{organization/repository}}
```
{% endraw %}