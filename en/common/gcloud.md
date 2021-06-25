---
layout: default
title: "gcloud"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcloud">
  <a href="/en/common/gcloud.html">gcloud</a> <a href="#gcloud"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The official CLI tool for Google Cloud Platform.
> More information: <https://cloud.google.com/sdk/gcloud>.

#### List all properties in one's active configuration:
```shell
gcloud config list
```
#### Log in to Google account:
```shell
gcloud auth login
```
#### Set the active project:
```shell
gcloud config set project {{project_name}}
```
#### SSH into a virtual machine instance:
```shell
gcloud compute ssh {{user}}@{{instance}} 
```
#### Display all Google Compute Engine instances in a project. Instances from all zones are listed by default:
```shell
gcloud compute instances list
```
#### Update a kubeconfig file with the appropriate credentials to point kubectl to a specific cluster in Google Kubernetes Engine:
```shell
gcloud container clusters get-credentials {{cluster_name}}
```
#### Update all gcloud CLI components:
```shell
gcloud components update
```
#### Show help for a given command:
```shell
gcloud help {{command}}
```
{% endraw %}