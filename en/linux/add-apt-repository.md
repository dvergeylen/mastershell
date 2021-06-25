---
layout: default
title: "add-apt-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="add-apt-repository">
  <a href="/en/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manages apt repository definitions.

#### Add a new apt repository:
```shell
add-apt-repository {{repository_spec}}
```
#### Remove an apt repository:
```shell
add-apt-repository --remove {{repository_spec}}
```
#### Update the package cache after adding a repository:
```shell
add-apt-repository --update {{repository_spec}}
```
#### Enable source packages:
```shell
add-apt-repository --enable-source {{repository_spec}}
```
{% endraw %}