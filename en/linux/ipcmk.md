---
layout: default
title: "ipcmk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipcmk">
  <a href="/en/linux/ipcmk.html">ipcmk</a> <a href="#ipcmk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create IPC (Inter-process Communication) resources.

#### Create a shared memory segment:
```shell
ipcmk --shmem {{segment_size_in_bytes}}
```
#### Create a semaphore:
```shell
ipcmk --semaphore {{element_size}}
```
#### Create a message queue:
```shell
ipcmk --queue
```
#### Create a shared memory segment with specific permissions (default is 0644):
```shell
ipcmk --shmem {{segment_size_in_bytes}} {{octal_permissons}}
```
{% endraw %}