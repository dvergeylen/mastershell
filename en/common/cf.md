---
layout: default
title: "cf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cf">
  <a href="/en/common/cf.html">cf</a> <a href="#cf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to manage apps and services on Cloud Foundry.
> More information: <https://docs.cloudfoundry.org>.

#### Push an app using the default settings:
```shell
cf push {{app_name}}
```
#### View the services available from your organization:
```shell
cf marketplace
```
#### Create a service instance:
```shell
cf create-service {{service}} {{plan}} {{service_name}}
```
#### Connect an application to a service:
```shell
cf bind-service {{app_name}} {{service_name}}
```
#### Run a script whose code is included in the app, but runs independently:
```shell
cf run-task {{app_name}} "{{script_command}}" --name {{task_name}}
```
#### Start an interactive SSH session with a VM hosting an app:
```shell
cf ssh {{app_name}}
```
#### View a dump of recent app logs:
```shell
cf logs {{app_name}} --recent
```
{% endraw %}