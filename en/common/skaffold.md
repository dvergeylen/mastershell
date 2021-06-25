---
layout: default
title: "skaffold"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="skaffold">
  <a href="/en/common/skaffold.html">skaffold</a> <a href="#skaffold"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool that facilitates continuous development for Kubernetes applications.
> More information: <https://skaffold.dev>.

#### Build the artifacts:
```shell
skaffold build -f {{skaffold.yaml}}
```
#### Build and deploy your app every time your code changes:
```shell
skaffold dev -f {{skaffold.yaml}}
```
#### Run a pipeline file:
```shell
skaffold run -f {{skaffold.yaml}}
```
#### Run a diagnostic on Skaffold:
```shell
skaffold diagnose -f {{skaffold.yaml}}
```
#### Deploy the artifacts:
```shell
skaffold deploy -f {{skaffold.yaml}}
```
{% endraw %}