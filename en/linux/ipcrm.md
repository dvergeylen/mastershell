---
layout: default
title: "ipcrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipcrm">
  <a href="/en/linux/ipcrm.html">ipcrm</a> <a href="#ipcrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete IPC (Inter-process Communication) resources.

#### Delete a shared memory segment by ID:
```shell
ipcrm --shmem-id {{shmem_id}}
```
#### Delete a shared memory segment by key:
```shell
ipcrm --shmem-key {{shmem_key}}
```
#### Delete an IPC queue by ID:
```shell
ipcrm --queue-id {{ipc_queue_id}}
```
#### Delete an IPC queue by key:
```shell
ipcrm --queue-key {{ipc_queue_key}}
```
#### Delete a semaphore by ID:
```shell
ipcrm --semaphore-id {{semaphore_id}}
```
#### Delete a semaphore by key:
```shell
ipcrm --semaphore-key {{semaphore_key}}
```
#### Delete all IPC resources:
```shell
ipcrm --all
```
{% endraw %}