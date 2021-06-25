---
layout: default
title: "choco feature"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-feature">
  <a href="/en/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with features with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-feature>.

#### Display a list of available features:
```shell
choco feature list
```
#### Enable a feature:
```shell
choco feature enable --name {{name}}
```
#### Disable a feature:
```shell
choco feature disable --name {{name}}
```
{% endraw %}