---
layout: default
title: "jhipster"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jhipster">
  <a href="/en/common/jhipster.html">jhipster</a> <a href="#jhipster"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web application generator using either monolithic or microservices architecture.
> More information: <https://www.jhipster.tech/>.

#### Generate a simple full-stack project (monolithic or microservices):
```shell
jhipster
```
#### Generate a simple frontend project:
```shell
jhipster --skip-server
```
#### Generate a simple backend project:
```shell
jhipster --skip-client
```
#### Apply latest JHipster updates to the project:
```shell
jhipster upgrade
```
#### Add a new entity to a generated project:
```shell
jhipster entity {{entity_name}}
```
#### Import a JDL file to configure your application (see: https://start.jhipster.tech/jdl-studio/):
```shell
jhipster import-jdl {{first_file.jh second_file.jh ... n_file.jh}}
```
#### Generate a CI/CD pipeline for your application:
```shell
jhipster ci-cd
```
#### Generate a Kubernetes configuration for your application:
```shell
jhipster kubernetes
```
{% endraw %}