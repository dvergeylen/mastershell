---
layout: default
title: "rbenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rbenv">
  <a href="/en/common/rbenv.html">rbenv</a> <a href="#rbenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to easily install Ruby versions and manage application environments.
> More information: <https://github.com/rbenv/rbenv>.

#### Install a Ruby version:
```shell
rbenv install {{version}}
```
#### Display a list of the latest stable versions for each Ruby:
```shell
rbenv install --list
```
#### Display a list of installed Ruby versions:
```shell
rbenv versions
```
#### Use a specific Ruby version across the whole system:
```shell
rbenv global {{version}}
```
#### Use a specific Ruby version for an application/project directory:
```shell
rbenv local {{version}}
```
#### Display the currently selected Ruby version:
```shell
rbenv version
```
#### Uninstall a Ruby version:
```shell
rbenv uninstall {{version}}
```
#### Display all Ruby versions that contain the specified executable:
```shell
rbenv whence {{executable}}
```
{% endraw %}