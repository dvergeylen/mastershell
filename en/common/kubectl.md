---
layout: default
title: "kubectl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubectl">
  <a href="/en/common/kubectl.html">kubectl</a> <a href="#kubectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for running commands against Kubernetes clusters.
> See also `kubectl describe` and other pages for additional information.
> More information: <https://kubernetes.io/docs/reference/kubectl/>.

#### List information about a resource with more details:
```shell
kubectl get {{pod|service|deployment|ingress|...}} -o wide
```
#### Update specified pod with the label 'unhealthy' and the value 'true':
```shell
kubectl label pods {{name}} unhealthy=true
```
#### List all resources with different types:
```shell
kubectl get all
```
#### Display resource (CPU/Memory/Storage) usage of nodes or pods:
```shell
kubectl top {{pod|node}}
```
#### Print the address of the master and cluster services:
```shell
kubectl cluster-info
```
#### Display an explanation of a specific field:
```shell
kubectl explain {{pods.spec.containers}}
```
#### Print the logs for a container in a pod or specified resource:
```shell
kubectl logs {{pod_name}}
```
#### Run command in an existing pod:
```shell
kubectl exec {{pod_name}} -- {{ls /}}
```
{% endraw %}