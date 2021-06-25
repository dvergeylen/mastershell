---
layout: default
title: "scoop bucket"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scoop-bucket">
  <a href="/en/windows/scoop-bucket.html">scoop bucket</a> <a href="#scoop-bucket"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage buckets: Git repositories containing files which describe how scoop installs applications.
> If Scoop doesn't know where the bucket is located its repository location must be specified.
> More information: <https://github.com/lukesampson/scoop/wiki/Buckets>.

#### List all buckets currently in use:
```shell
scoop bucket list
```
#### List all known buckets:
```shell
scoop bucket known
```
#### Add a known bucket by its name:
```shell
scoop bucket add {{name}}
```
#### Add an unknown bucket by its name and Git repository URL:
```shell
scoop bucket add {{name}} {{https://example.com/repository.git}}
```
#### Remove a bucket by its name:
```shell
scoop bucket rm {{name}}
```
{% endraw %}