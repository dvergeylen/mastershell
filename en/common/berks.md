---
layout: default
title: "berks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="berks">
  <a href="/en/common/berks.html">berks</a> <a href="#berks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chef cookbook dependency manager.
> More information: <https://docs.chef.io/berkshelf.html>.

#### Install cookbook dependencies into a local repo:
```shell
berks install
```
#### Update a specific cookbook and its dependencies:
```shell
berks update {{cookbook}}
```
#### Upload a cookbook to the Chef server:
```shell
berks upload {{cookbook}}
```
#### View the dependencies of a cookbook:
```shell
berks contingent {{cookbook}}
```
{% endraw %}