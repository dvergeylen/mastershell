---
layout: default
title: "oc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="oc">
  <a href="/en/common/oc.html">oc</a> <a href="#oc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The OpenShift Container Platform CLI.
> Allows for application and container management.
> More information: <https://docs.openshift.com/container-platform/3.11/cli_reference/get_started_cli.html>.

#### Log in to the OpenShift Container Platform server:
```shell
oc login
```
#### Create a new project:
```shell
oc new-project {{project_name}}
```
#### Switch to an existing project:
```shell
oc project {{project_name}}
```
#### Add a new application to a project:
```shell
oc new-app {{repo_url}} --name {{application}}
```
#### Open a remote shell session to a container:
```shell
oc rsh {{pod_name}}
```
#### List pods in a project:
```shell
oc get pods
```
#### Log out from the current session:
```shell
oc logout
```
{% endraw %}