---
layout: default
title: "molecule"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="molecule">
  <a href="/en/common/molecule.html">molecule</a> <a href="#molecule"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Molecule helps testing ansible roles.
> More information: <https://molecule.readthedocs.io>.

#### Create a new ansible role:
```shell
molecule init role --role-name {{role_name}}
```
#### Run tests:
```shell
molecule test
```
#### Start the instance:
```shell
molecule create
```
#### Configure the instance:
```shell
molecule converge
```
#### Log in into the instance:
```shell
molecule login
```
{% endraw %}