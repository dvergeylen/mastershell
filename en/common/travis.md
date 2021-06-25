---
layout: default
title: "travis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="travis">
  <a href="/en/common/travis.html">travis</a> <a href="#travis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client to interface with Travis CI.
> More information: <https://github.com/travis-ci/travis.rb>.

#### Display the client version:
```shell
travis version
```
#### Authenticate the CLI client against the server, using an authentication token:
```shell
travis login
```
#### List repositories the user has permissions on:
```shell
travis repos
```
#### Encrypt values in `.travis.yml`:
```shell
travis encrypt {{token}}
```
#### Generate a `.travis.yml` file and enable the project:
```shell
travis init
```
{% endraw %}