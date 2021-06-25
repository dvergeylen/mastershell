---
layout: default
title: "kops"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kops">
  <a href="/en/common/kops.html">kops</a> <a href="#kops"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, destroy, upgrade and maintain Kubernetes clusters from the command-line.
> More information: <https://github.com/kubernetes/kops/>.

#### Create a cluster from the configuration specification:
```shell
kops create cluster -f {{cluster_name.yaml}}
```
#### Create a new ssh public key:
```shell
kops create secret sshpublickey {{key_name}} -i {{~/.ssh/id_rsa.pub}}
```
#### Export the cluster configuration to the `~/.kube/config` file:
```shell
kops export kubecfg {{cluster_name}}
```
#### Get the cluster configuration as yaml:
```shell
kops get cluster {{cluster_name}} -o yaml
```
#### Delete a cluster:
```shell
kops delete cluster {{cluster_name}} --yes
```
{% endraw %}