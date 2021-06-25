---
layout: default
title: "rbac-lookup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rbac-lookup">
  <a href="/en/common/rbac-lookup.html">rbac-lookup</a> <a href="#rbac-lookup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find roles and cluster roles attached to any user, service account or group name in your Kubernetes cluster.
> More information: <https://github.com/reactiveops/rbac-lookup>.

#### View all RBAC bindings:
```shell
rbac-lookup
```
#### View RBAC bindings that match a given expression:
```shell
rbac-lookup {{search_term}}
```
#### View all RBAC bindings along with the source role binding:
```shell
rbac-lookup -o wide
```
#### View all RBAC bindings filtered by subject:
```shell
rbac-lookup -k {{user|group|serviceaccount}}
```
#### View all RBAC bindings along with IAM roles (if you are using GKE):
```shell
rbac-lookup --gke
```
{% endraw %}