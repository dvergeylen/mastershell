---
layout: default
title: "tox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tox">
  <a href="/en/common/tox.html">tox</a> <a href="#tox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automate Python testing across multiple Python versions.
> Use tox.ini to configure environments and test command.
> More information: <https://github.com/tox-dev/tox>.

#### Run tests on all test environments:
```shell
tox
```
#### Create a `tox.ini` configuration:
```shell
tox-quickstart
```
#### List the available environments:
```shell
tox --listenvs-all
```
#### Run tests on a specific environment (e.g. python 3.6):
```shell
tox -e {{py36}}
```
#### Force the virtual environment to be recreated:
```shell
tox --recreate -e {{py27}}
```
{% endraw %}