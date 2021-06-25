---
layout: default
title: "ndctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ndctl">
  <a href="/en/linux/ndctl.html">ndctl</a> <a href="#ndctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for managing Non-Volatile DIMMs.

#### Create an 'fsdax' mode namespace:
```shell
ndctl create-namespace --mode={{fsdax}}
```
#### Change the mode of a namespace to 'raw':
```shell
ndctl create-namespace --reconfigure={{namespaceX.Y}} --mode={{raw}}
```
#### Check a sector mode namespace for consistency, and repair if needed:
```shell
ndctl check-namespace --repair {{namespaceX.Y}}
```
#### List all namespaces, regions, and buses (including disabled ones):
```shell
ndctl list --namespaces --regions --buses --idle
```
#### List a specific namespace and include lots of additional information:
```shell
ndctl list -vvv --namespace={{namespaceX.Y}}
```
#### Run a monitor to watch for SMART health events for NVDIMMs on the 'ACPI.NFIT' bus:
```shell
ndctl monitor --bus={{ACPI.NFIT}}
```
#### Remove a namespace (when applicable) or reset it to an initial state:
```shell
ndctl destroy-namespace --force {{namespaceX.Y}}
```
{% endraw %}