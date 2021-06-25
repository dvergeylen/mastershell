---
layout: default
title: "k8sec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="k8sec">
  <a href="/en/common/k8sec.html">k8sec</a> <a href="#k8sec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface tool to manage Kubernetes secrets.
> More information: <https://github.com/dtan4/k8sec>.

#### List all secrets:
```shell
k8sec list
```
#### List a specific secret as a base64-encoded string:
```shell
k8sec list {{secret_name}} --base64
```
#### Set a secret's value:
```shell
k8sec set {{secret_name}} {{key=value}}
```
#### Set a base64-encoded value:
```shell
k8sec set --base64 {{secret_name}} {{key=encoded_value}}
```
#### Unset a secret:
```shell
k8sec unset {{secret_name}}
```
#### Load secrets from a file:
```shell
k8sec load -f {{path/to/file}} {{secret_name}}
```
#### Dump secrets to a file:
```shell
k8sec dump -f {{path/to/file}} {{secret_name}}
```
{% endraw %}