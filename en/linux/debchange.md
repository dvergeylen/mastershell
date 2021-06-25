---
layout: default
title: "debchange"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debchange">
  <a href="/en/linux/debchange.html">debchange</a> <a href="#debchange"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for maintenance of the debian/changelog file in a Debian source package.
> More information: <https://manpages.debian.org/debchange>.

#### Add a new version for a non-maintainer upload to the changelog:
```shell
debchange --nmu
```
#### Add a changelog entry to the current version:
```shell
debchange --append
```
#### Add a changelog entry to close the bug with specified ID:
```shell
debchange --closes {{bug_id}}
```
{% endraw %}