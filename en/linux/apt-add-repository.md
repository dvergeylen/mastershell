---
layout: default
title: "apt-add-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-add-repository">
  <a href="/en/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manages apt repository definitions.
> More information: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Add a new apt repository:
```shell
apt-add-repository {{repository_spec}}
```
#### Remove an apt repository:
```shell
apt-add-repository --remove {{repository_spec}}
```
#### Update the package cache after adding a repository:
```shell
apt-add-repository --update {{repository_spec}}
```
#### Enable source packages:
```shell
apt-add-repository --enable-source {{repository_spec}}
```
{% endraw %}