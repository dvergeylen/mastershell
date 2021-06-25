---
layout: default
title: "hadolint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hadolint">
  <a href="/en/common/hadolint.html">hadolint</a> <a href="#hadolint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dockerfile linter.
> More information: <https://github.com/hadolint/hadolint>.

#### Lint a Dockerfile:
```shell
hadolint {{path/to/Dockerfile}}
```
#### Lint a Dockerfile, displaying the output in JSON format:
```shell
hadolint --format {{json}} {{path/to/Dockerfile}}
```
#### Lint a Dockerfile, displaying the output in a specific format:
```shell
hadolint --format {{tty|json|checkstyle|codeclimate|codacy}} {{path/to/Dockerfile}}
```
#### Lint a Dockerfile ignoring specific rules:
```shell
hadolint --ignore {{DL3006}} --ignore {{DL3008}} {{path/to/Dockerfile}}
```
#### Lint multiple Dockerfiles using specific trusted registries:
```shell
hadolint --trusted-registry {{docker.io}} --trusted-registry {{example.com}}:{{5000}} {{path/to/Dockerfile}} {{path/to/another/Dockerfile}}
```
{% endraw %}