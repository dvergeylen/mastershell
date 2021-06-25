---
layout: default
title: "secrethub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="secrethub">
  <a href="/en/common/secrethub.html">secrethub</a> <a href="#secrethub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to keep secrets out of config files.
> More information: <https://secrethub.io>.

#### Print a secret to stdout:
```shell
secrethub read {{path/to/secret}}
```
#### Generate a random value and store it as a new or updated secret:
```shell
secrethub generate {{path/to/secret}}
```
#### Store a value from the clipboard as a new or updated secret:
```shell
secrethub write --clip {{path/to/secret}}
```
#### Store a value supplied on stdin as a new or updated secret:
```shell
echo "{{secret_value}}" | secrethub write {{path/to/secret}}
```
#### Audit a repository or secret:
```shell
secrethub audit {{path/to/repo_or_secret}}
```
{% endraw %}