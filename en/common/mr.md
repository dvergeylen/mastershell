---
layout: default
title: "mr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mr">
  <a href="/en/common/mr.html">mr</a> <a href="#mr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage all of your version control repositories at once.
> More information: <https://myrepos.branchable.com>.

#### Register a repository:
```shell
mr register
```
#### Update repositories in 5 concurrent jobs:
```shell
mr -j{{5}} update
```
#### Print the status of all repositories:
```shell
mr status
```
#### Checkout all repositories to the latest version:
```shell
mr checkout
```
{% endraw %}