---
layout: default
title: "dexter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dexter">
  <a href="/en/common/dexter.html">dexter</a> <a href="#dexter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for authenticating the kubectl users with OpenId Connect.
> More information: <https://github.com/gini/dexter>.

#### Create and authenticate a user with Google OIDC:
```shell
dexter auth -i {{client_id}} -s {{client_secret}}
```
#### Override the default kube config location:
```shell
dexter auth -i {{client_id}} -s {{client_secret}} --kube-config {{sample/config}}
```
{% endraw %}