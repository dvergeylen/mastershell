---
layout: default
title: "git credential"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-credential">
  <a href="/en/common/git-credential.html">git credential</a> <a href="#git-credential"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retrieve and store user credentials.
> More information: <https://git-scm.com/docs/git-credential>.

#### Display credential information, retrieving the username and password from configuration files:
```shell
echo "{{url=http://example.com}}" | git credential fill
```
#### Send credential information to all configured credential helpers to store for later use:
```shell
echo "{{url=http://example.com}}" | git credential approve
```
#### Erase the specified credential information from all the configured credential helpers:
```shell
echo "{{url=http://example.com}}" | git credential reject
```
{% endraw %}