---
layout: default
title: "larasail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="larasail">
  <a href="/en/linux/larasail.html">larasail</a> <a href="#larasail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI tool for managing Laravel on Digital Ocean servers.
> More information: <https://github.com/thedevdojo/larasail>.

#### Set up the server with Laravel dependencies using the default PHP version:
```shell
larasail setup
```
#### Set up the server with Laravel dependencies using a specific PHP version:
```shell
larasail setup {{php71}}
```
#### Add a new Laravel site:
```shell
larasail host {{domain}} {{path/to/site_directory}}
```
#### Retrieve the Larasail user password:
```shell
larasail pass
```
#### Retrieve the Larasail MySQL password:
```shell
larasail mysqlpass
```
{% endraw %}